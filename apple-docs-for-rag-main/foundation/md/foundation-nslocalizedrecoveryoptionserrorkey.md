

- Foundation
-  NSLocalizedRecoveryOptionsErrorKey 

Global Variable

# NSLocalizedRecoveryOptionsErrorKey

The corresponding value is an array containing the localized titles of buttons appropriate for displaying in an alert panel.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSLocalizedRecoveryOptionsErrorKey: String
```

## Discussion

The first string is the title of the right-most and default button, the second the one to the left, and so on. The recovery options should be appropriate for the recovery suggestion returned by localizedRecoverySuggestion.

## See Also

### Constants

let NSURLErrorKey: String

The corresponding value is an `NSURL` object.

let NSFilePathErrorKey: String

Contains the file path of the error.

let NSHelpAnchorErrorKey: String

The corresponding value is an `NSString` containing the localized help corresponding to the help button. See helpAnchor for more information.

let NSLocalizedDescriptionKey: String

The corresponding value is a localized string representation of the error that, if present, will be returned by localizedDescription.

let NSLocalizedFailureErrorKey: String

let NSLocalizedFailureReasonErrorKey: String

The corresponding value is a localized string representation containing the reason for the failure that, if present, will be returned by localizedFailureReason.

let NSLocalizedRecoverySuggestionErrorKey: String

The corresponding value is a string containing the localized recovery suggestion for the error.

let NSRecoveryAttempterErrorKey: String

The corresponding value is an object that conforms to the NSErrorRecoveryAttempting informal protocol.

let NSStringEncodingErrorKey: String

The corresponding value is an `NSNumber` object containing the `NSStringEncoding` value.

let NSUnderlyingErrorKey: String

The corresponding value is an error that was encountered in an underlying implementation and caused the error that the receiver represents to occur.

let NSDebugDescriptionErrorKey: String

let NSMultipleUnderlyingErrorsKey: String

