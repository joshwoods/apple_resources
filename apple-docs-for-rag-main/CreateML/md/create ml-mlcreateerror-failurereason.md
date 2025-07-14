

- Create ML
- MLCreateError
-  failureReason 

Instance Property

# failureReason

A localized, human-readable reason behind the failure, if applicable.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var failureReason: String? { get }
```

## See Also

### Describing errors in a user interface

static var errorDomain: String

Default domain of the error.

var localizedDescription: String

Retrieve the localized description for this error.

var errorCode: Int

The numeric code of this error.

var errorUserInfo: [String : Any]

A dictionary that provides additional information about the error.

var errorDescription: String?

A localized, human-readable description of the error and why it occurred, if applicable.

var helpAnchor: String?

A localized message providing “help” text if the user requests help.

var recoverySuggestion: String?

A localized message describing how one might recover from the failure.

