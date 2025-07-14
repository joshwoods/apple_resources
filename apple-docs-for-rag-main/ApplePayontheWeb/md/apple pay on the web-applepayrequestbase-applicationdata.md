

- Apple Pay on the Web
- ApplePayRequestBase
-  applicationData 

Instance Property

# applicationData

Application-specific data or state you can add to support your app.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
DOMString applicationData;
```

## Discussion

Use this property for additional data as may be appropriate for your app—for example, a shopping cart identifier or an order number.

The signed payment data (the paymentData property of PKPaymentToken) includes a hash of this data. You’re responsible for sending the full application data to your server, if needed.

