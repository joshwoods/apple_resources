

- Foundation
- NSError
-  localizedRecoverySuggestion 

Instance Property

# localizedRecoverySuggestion

A string containing the localized recovery suggestion for the error.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var localizedRecoverySuggestion: String? { get }
```

## Discussion

The object in the user info dictionary for the key NSLocalizedRecoverySuggestionErrorKey. If the user info dictionary doesn’t contain a value for NSLocalizedRecoverySuggestionErrorKey, this property is `nil`.

The returned string is suitable for displaying as the secondary message in an alert panel.

## See Also

### Getting a Localized Error Description

var localizedDescription: String

A string containing the localized description of the error.

var localizedRecoveryOptions: [String]?

An array containing the localized titles of buttons appropriate for displaying in an alert panel.

var localizedFailureReason: String?

A string containing the localized explanation of the reason for the error.

