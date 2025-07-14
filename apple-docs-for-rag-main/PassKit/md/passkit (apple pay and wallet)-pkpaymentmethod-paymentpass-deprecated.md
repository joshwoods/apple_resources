

- PassKit (Apple Pay and Wallet)
- PKPaymentMethod
-  paymentPass Deprecated

Instance Property

# paymentPass

The accompanying payment pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 3.0–9.0Deprecated

``` source
@NSCopying
var paymentPass: PKPaymentPass? { get }
```

Deprecated

Use secureElementPass instead.

## Discussion

If your app has an association with the pass that is funding the payment, this property contains information about that pass; otherwise, it’s `nil`.

Use this property to detect your brand of credit and debit cards. For example, you can provide a discount if the user pays using your store-branded credit card.

Note

To be able to access the pass, the issuer must add your App ID to the pass when it provisions it. To add your App ID to these passes, contact the bank that issues your cards or the person who manages your cobrand program.

## See Also

### Getting the pass

var secureElementPass: PKSecureElementPass?

The accompanying Secure Element pass.

