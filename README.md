The payment flow assumed is :
  1. User would get a order_id from other microservice(order-service) and pass it to payment service.
  2. /payments - returns a payment link in response, FE will redirect user to the link for payment
  3. Once the transaction is completed, a webhook is configured in the Payment Gateway, db can be updated accordingly.


Design Pattern:
Strategy: 
  Strategy Pattern is used to choose a payment gateway.


