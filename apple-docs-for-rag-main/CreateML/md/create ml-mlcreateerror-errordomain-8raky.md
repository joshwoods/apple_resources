

- Create ML
- MLCreateError
-  errorDomain 

Type Property

# errorDomain

Default domain of the error.

Create MLFoundationiOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var errorDomain: String { get }
```

## See Also

### Describing errors in a user interface

var localizedDescription: String

Retrieve the localized description for this error.

var errorCode: Int

The numeric code of this error.

var errorUserInfo: [String : Any]

A dictionary that provides additional information about the error.

var errorDescription: String?

A localized, human-readable description of the error and why it occurred, if applicable.

var failureReason: String?

A localized, human-readable reason behind the failure, if applicable.

var helpAnchor: String?

A localized message providing “help” text if the user requests help.

var recoverySuggestion: String?

A localized message describing how one might recover from the failure.

