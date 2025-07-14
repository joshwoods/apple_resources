

- StoreKit
- SKPaymentTransactionObserver
-  paymentQueue(\_:updatedDownloads:) Deprecated

Instance Method

# paymentQueue(\_:updatedDownloads:)

Tells the observer that the payment queue has updated one or more download objects.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
optional func paymentQueue(
    _ queue: SKPaymentQueue,
    updatedDownloads downloads: [SKDownload]
)
```

Deprecated

Hosted content is no longer supported

## Parameters 

`queue`  

The payment queue that updated the downloads.

`downloads`  

The download objects that were updated.

## Mentioned in 

Unlocking purchased content

## Discussion

When a download object is updated, its downloadState property describes how it changed.

