

- StoreKit
- SKPaymentTransaction
-  downloads Deprecated

Instance Property

# downloads

An array of download objects representing the downloadable content associated with the transaction.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var downloads: [SKDownload] { get }
```

Deprecated

Hosted content is no longer supported

## Mentioned in 

Unlocking purchased content

## Discussion

The contents of this property are undefined except when transactionState is set to SKPaymentTransactionState.purchased. The SKDownload objects stored in this property must be used to download the transaction’s content before the transaction is finished. After the transaction is finished, the download objects are no longer queueable.

