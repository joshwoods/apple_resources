

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  isSuppressingAutomaticPassPresentation() 

Type Method

# isSuppressingAutomaticPassPresentation()

Returns a Boolean value that indicates whether the system suppresses the automatic presentation of Apple Pay passes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 10.2+

``` source
class func isSuppressingAutomaticPassPresentation() -> Bool
```

## Return Value

true if the system suppresses Apple Pay passes; otherwise, false.

## See Also

### Presenting and suppressing passes

func present(PKSecureElementPass)

Presents a Secure Element pass.

class func requestAutomaticPassPresentationSuppression(responseHandler: (PKAutomaticPassPresentationSuppressionResult) -> Void) -> PKSuppressionRequestToken

Prevents the device from automatically displaying the Apple Pay interface.

enum PKAutomaticPassPresentationSuppressionResult

The result of an attempt to suppress automatic pass presentation.

class func endAutomaticPassPresentationSuppression(withRequestToken: PKSuppressionRequestToken)

Reenables the automatic display of the Apple Pay interface.

typealias PKSuppressionRequestToken

A token that represents a request to suppress the automatic presentation of payment passes.

