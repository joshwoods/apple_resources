

- PassKit (Apple Pay and Wallet)
-  PKAutomaticPassPresentationSuppressionResult 

Enumeration

# PKAutomaticPassPresentationSuppressionResult

The result of an attempt to suppress automatic pass presentation.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 10.2+

``` source
enum PKAutomaticPassPresentationSuppressionResult
```

## Topics

### Constants

case notSupported

The device doesn’t support the suppression of automatic pass presentation.

case alreadyPresenting

The device is already presenting passes.

case denied

The user prevented the suppression, or an internal error occurred.

case cancelled

The system canceled the suppression before calling the response handler.

case success

Suppression of automatic presentation successful.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Presenting and suppressing passes

func present(PKSecureElementPass)

Presents a Secure Element pass.

class func isSuppressingAutomaticPassPresentation() -> Bool

Returns a Boolean value that indicates whether the system suppresses the automatic presentation of Apple Pay passes.

class func requestAutomaticPassPresentationSuppression(responseHandler: (PKAutomaticPassPresentationSuppressionResult) -> Void) -> PKSuppressionRequestToken

Prevents the device from automatically displaying the Apple Pay interface.

class func endAutomaticPassPresentationSuppression(withRequestToken: PKSuppressionRequestToken)

Reenables the automatic display of the Apple Pay interface.

typealias PKSuppressionRequestToken

A token that represents a request to suppress the automatic presentation of payment passes.

