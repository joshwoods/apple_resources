

- StoreKit
- SKMutablePayment
-  applicationUsername Deprecated

Instance Property

# applicationUsername

A string that associates the transaction with a user account on your service.

iOS 7.0–18.0DeprecatediPadOS 7.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.9–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var applicationUsername: String? { get set }
```

Deprecated

Create a Product.PurchaseOption.appAccountToken to use in Product.purchase(confirmIn:options:)

## Mentioned in 

Implementing promotional offers in your app

Restoring purchased products

Generating a signature for promotional offers

## Discussion

Consider assigning a UUID to the applicationUsername property. When this value is a UUID, the App Store server stores it as an appAccountToken. In this scenario, the following happens:

- In the App Store Server API, the JWSTransactionDecodedPayload object returns the applicationUsername value in the appAccountToken field.

- In App Store Server Notifications, the JWSTransactionDecodedPayload object returns the applicationUsername value in the appAccountToken field.

- When you call the verifyReceipt endpoint to verify an App Store receipt, the App Store server returns the applicationUsername value in the app_account_token field of the responseBody.Latest_receipt_info.

The sample code below shows how to assign a UUID value to applicationUsername. You may choose to generate the UUID on your server. Assign the value before adding the payment to the payment queue.

- Swift
- Objective-C

```
let payment = SKMutablePayment(product: product)
payment.applicationUsername = uuidString

SKPaymentQueue.default().add(payment)
```

```
SKMutablePayment *payment = [SKMutablePayment paymentWithProduct:product];
payment.applicationUsername = uuidString;

[[SKPaymentQueue defaultQueue] addPayment:payment];
```

If you don’t assign a UUID string value to applicationUsername, the App Store server doesn’t persist the value. The value won’t appear in the app_account_token fields in notifications or receipts.

Important

An applicationUsername property that isn’t a UUID isn’t guaranteed to persist between the time when you add the payment transaction to the queue and when the queue updates the transaction.

## See Also

### Getting and Setting Attributes

var productIdentifier: String

A string that identifies a product that can be purchased from within your app.

Deprecated

var quantity: Int

The number of items the user wants to purchase.

Deprecated

var requestData: Data?

Reserved for future use.

Deprecated

