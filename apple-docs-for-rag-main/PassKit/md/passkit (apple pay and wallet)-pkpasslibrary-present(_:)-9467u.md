

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  present(\_:) 

Instance Method

# present(\_:)

Presents a Secure Element pass.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.12+visionOS 1.0+

``` source
func present(_ pass: PKSecureElementPass)
```

## Parameters 

`pass`  

The Secure Element pass to present.

## Discussion

Your app can only present provisioned passes. The library must contain `pass`. Otherwise, calling this method has no effect.

## See Also

### Presenting and suppressing passes

class func isSuppressingAutomaticPassPresentation() -> Bool

Returns a Boolean value that indicates whether the system suppresses the automatic presentation of Apple Pay passes.

class func requestAutomaticPassPresentationSuppression(responseHandler: (PKAutomaticPassPresentationSuppressionResult) -> Void) -> PKSuppressionRequestToken

Prevents the device from automatically displaying the Apple Pay interface.

enum PKAutomaticPassPresentationSuppressionResult

The result of an attempt to suppress automatic pass presentation.

class func endAutomaticPassPresentationSuppression(withRequestToken: PKSuppressionRequestToken)

Reenables the automatic display of the Apple Pay interface.

typealias PKSuppressionRequestToken

A token that represents a request to suppress the automatic presentation of payment passes.

