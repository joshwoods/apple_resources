

- StoreKit
- ExternalPurchase
- ExternalPurchase.NoticeResult
-  ExternalPurchase.NoticeResult.continuedWithExternalPurchaseToken(token:) 

Case

# ExternalPurchase.NoticeResult.continuedWithExternalPurchaseToken(token:)

Describes when people chose to continue to view external purchases, and provides the external purchase token.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
case continuedWithExternalPurchaseToken(token: String)
```

## Parameters 

`token`  

The external purchase token.

## Mentioned in 

Receiving and decoding external purchase tokens

## Discussion

When your app calls presentNoticeSheet() and it results in this value: ExternalPurchase.NoticeResult.continuedWithExternalPurchaseToken(token:), your app can proceed to present external purchases.

Important

Record and use the token to report the customer’s external purchases to Apple. For more information, see External Purchase Server API.

\`\`

## See Also

### Getting notice sheet results

case cancelled

Describes when people chose to cancel and not view external purchases.

