

- PassKit (Apple Pay and Wallet)
-  PKSuppressionRequestToken 

Type Alias

# PKSuppressionRequestToken

A token that represents a request to suppress the automatic presentation of payment passes.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
typealias PKSuppressionRequestToken = Int
```

## Discussion

You receive a suppression request token when you begin suppressing the automatic presentation of passes. Use the token to end the suppression and reenable Apple Pay.

## See Also

### Presenting and suppressing passes

func present(PKSecureElementPass)

Presents a Secure Element pass.

class func isSuppressingAutomaticPassPresentation() -> Bool

Returns a Boolean value that indicates whether the system suppresses the automatic presentation of Apple Pay passes.

class func requestAutomaticPassPresentationSuppression(responseHandler: (PKAutomaticPassPresentationSuppressionResult) -> Void) -> PKSuppressionRequestToken

Prevents the device from automatically displaying the Apple Pay interface.

enum PKAutomaticPassPresentationSuppressionResult

The result of an attempt to suppress automatic pass presentation.

class func endAutomaticPassPresentationSuppression(withRequestToken: PKSuppressionRequestToken)

Reenables the automatic display of the Apple Pay interface.

