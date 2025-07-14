

- PassKit (Apple Pay and Wallet)
- PKAutomaticPassPresentationSuppressionResult
-  PKAutomaticPassPresentationSuppressionResult.alreadyPresenting 

Case

# PKAutomaticPassPresentationSuppressionResult.alreadyPresenting

The device is already presenting passes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+watchOS 10.2+

``` source
case alreadyPresenting
```

## Discussion

The device is unable to suppress automatic presentation of passes.

## See Also

### Constants

case notSupported

The device doesn’t support the suppression of automatic pass presentation.

case denied

The user prevented the suppression, or an internal error occurred.

case cancelled

The system canceled the suppression before calling the response handler.

case success

Suppression of automatic presentation successful.

