

- Foundation
-  ErrorUserInfoKey 

Structure

# ErrorUserInfoKey

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct ErrorUserInfoKey
```

## Topics

### Type Properties

static let NSURLErrorKey: ErrorUserInfoKeyDeprecated

static let filePathErrorKey: ErrorUserInfoKeyDeprecated

static let helpAnchorErrorKey: ErrorUserInfoKeyDeprecated

static let localizedDescriptionKey: ErrorUserInfoKeyDeprecated

static let localizedFailureReasonErrorKey: ErrorUserInfoKeyDeprecated

static let localizedRecoveryOptionsErrorKey: ErrorUserInfoKeyDeprecated

static let localizedRecoverySuggestionErrorKey: ErrorUserInfoKeyDeprecated

static let recoveryAttempterErrorKey: ErrorUserInfoKeyDeprecated

static let stringEncodingErrorKey: ErrorUserInfoKeyDeprecated

static let underlyingErrorKey: ErrorUserInfoKeyDeprecated

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Providing Error User Info

class func setUserInfoValueProvider(forDomain: String, provider: ((any Error, String) -> Any?)?)

Specifies a block to call when the corresponding property is not present in the user info dictionary.

class func userInfoValueProvider(forDomain: String) -> ((any Error, String) -> Any?)?

Returns any user info provider specified for a given error domain.

typealias UserInfoKey

These keys may exist in the user info dictionary.

