The payment flow assumed is :
1. User would get a order_id from other service and pass it to payment service.
2. /payments - returns a payment link, FE will redirect user to the link for payment
3. Once the payment is successful a webhook is configured which will called from the payment gateway and db can be updated accordingly.
