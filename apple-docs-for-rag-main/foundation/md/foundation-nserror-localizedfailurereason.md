

- Foundation
- NSError
-  localizedFailureReason 

Instance Property

# localizedFailureReason

A string containing the localized explanation of the reason for the error.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var localizedFailureReason: String? { get }
```

## Discussion

The object in the user info dictionary for the key NSLocalizedFailureReasonErrorKey.

## See Also

### Related Documentation

var domain: String

A string containing the error domain.

var code: Int

The error code.

var userInfo: [String : Any]

The user info dictionary.

### Getting a Localized Error Description

var localizedDescription: String

A string containing the localized description of the error.

var localizedRecoveryOptions: [String]?

An array containing the localized titles of buttons appropriate for displaying in an alert panel.

var localizedRecoverySuggestion: String?

A string containing the localized recovery suggestion for the error.

