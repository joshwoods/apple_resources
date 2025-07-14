

- App Store Server Notifications
-  appAccountToken 

Type

# appAccountToken

A UUID that associates the transaction with a customer on your service.

App Store Server Notifications 2.0+

``` source
uuid appAccountToken
```

## Mentioned in 

App Store Server Notifications changelog

## Discussion

When a customer initiates an in-app purchase, your app may create an appAccountToken(_:) and send it to the App Store. The App Store returns the same value in appAccountToken in the transaction information after the customer completes the purchase.

If you’re using the Original API for In-App Purchase and provide a UUID in the applicationUsername property, then the appAccountToken field contains that value.

