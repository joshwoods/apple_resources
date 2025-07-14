

- Apple Pay on the Web
- ApplePayPaymentRequest
-  applicationData 

Instance Property

# applicationData

A Base64-encoded string for application-specific data.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString applicationData;
```

## Discussion

Use this property to contain additional data as may be appropriate for your website. For example, the application data may be a shopping cart identifier or an order number that your back end needs to identify this transaction.

You’re responsible for sending the full application data to your server, if needed.

Important

If you use RegisterMerchantRequest in the Apple Pay Web Merchant Registration API to register merchants, you must include the merchant domain in applicationData. The payment service provider can use the domain in applicationData to ensure they know which merchant the payment token is for. The payment service provider uses the value in applicationData in a step necessary to validate the payment data. For more information, see Payment token format reference.

The applicationData string must be Base64-encoded; otherwise, the system ignores it.

