

- FamilyControls
- FamilyControlsError
-  errorDescription 

Instance Property

# errorDescription

A nonlocalized description of the error, suitable for debugging.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 13.0+

``` source
var errorDescription: String? { get }
```

## See Also

### Error Data

var localizedDescription: String

Retrieve the localized description for this error.

var failureReason: String?

A localized message describing the reason for the failure.

var recoverySuggestion: String?

A localized message describing how one might recover from the failure.

var helpAnchor: String?

A localized message providing “help” text if the user requests help.

