

- Foundation
- NSError
-  localizedRecoveryOptions 

Instance Property

# localizedRecoveryOptions

An array containing the localized titles of buttons appropriate for displaying in an alert panel.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var localizedRecoveryOptions: [String]? { get }
```

## Discussion

The object in the user info dictionary for the key NSLocalizedRecoveryOptionsErrorKey. If the user info dictionary doesn’t contain a value for NSLocalizedRecoveryOptionsErrorKey, this property is `nil`.

The first string is the title of the right-most and default button, the second the one to the left of that, and so on. The recovery options should be appropriate for the localizedRecoverySuggestion property. If the user info dictionary doesn’t contain a value for NSLocalizedRecoveryOptionsErrorKey, only an OK button is displayed.

## See Also

### Getting a Localized Error Description

var localizedDescription: String

A string containing the localized description of the error.

var localizedRecoverySuggestion: String?

A string containing the localized recovery suggestion for the error.

var localizedFailureReason: String?

A string containing the localized explanation of the reason for the error.

