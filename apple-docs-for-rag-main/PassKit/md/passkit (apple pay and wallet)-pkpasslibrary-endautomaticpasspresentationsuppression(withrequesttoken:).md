

- PassKit (Apple Pay and Wallet)
- PKPassLibrary
-  endAutomaticPassPresentationSuppression(withRequestToken:) 

Type Method

# endAutomaticPassPresentationSuppression(withRequestToken:)

Reenables the automatic display of the Apple Pay interface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.12+visionOS 1.0+watchOS 10.2+

``` source
class func endAutomaticPassPresentationSuppression(withRequestToken requestToken: PKSuppressionRequestToken)
```

## Parameters 

`requestToken`  

The token you receive when you call the PKPassLibrary method. If you pass in an invalid request token, the system ignores the end request.

## Discussion

This method reenables the automatic presentation of Apple Pay passes when the device detects a compatible reader.

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

typealias PKSuppressionRequestToken

A token that represents a request to suppress the automatic presentation of payment passes.

