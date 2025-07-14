

- StoreKit
- ExternalPurchase
- ExternalPurchase.NoticeResult
-  ExternalPurchase.NoticeResult.cancelled 

Case

# ExternalPurchase.NoticeResult.cancelled

Describes when people chose to cancel and not view external purchases.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
case cancelled
```

## Discussion

If your app’s call to presentNoticeSheet() results in this value, you must not show external purchases.

## See Also

### Getting notice sheet results

case continuedWithExternalPurchaseToken(token: String)

Describes when people chose to continue to view external purchases, and provides the external purchase token.

