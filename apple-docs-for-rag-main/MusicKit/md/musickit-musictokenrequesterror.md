

- MusicKit
-  MusicTokenRequestError 

Enumeration

# MusicTokenRequestError

An error that the token provider or music requests can throw upon requesting any token necessary for accessing Apple Music API.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum MusicTokenRequestError
```

## Topics

### Enumeration Cases

case developerTokenRequestFailed

An error that indicates a failure in the process of fetching a developer token for the current app.

case permissionDenied

An error that occurs when the user doesn’t consent for the current app to access their Apple Music data.

case privacyAcknowledgementRequired

An error that occurs when the user needs to acknowledge the most recent privacy policy.

case unknown

An error indicating the ocurrence of an unknown or unexpected error.

case userNotSignedIn

An error that occurs when the user isn’t signed in with an Apple Music account.

case userTokenRequestFailed

An error that indicates a failure in the process of fetching a user token.

case userTokenRevoked

An error that occurs when the user revokes permission for the current app to access their Apple Music data.

### Initializers

init?(rawValue: String)

Creates a new instance with the specified raw value.

### Instance Properties

var description: String

A textual representation of this instance.

var errorDescription: String?

A localized message describing what error occurred.

var failureReason: String?

A localized message describing the reason for the failure.

var helpAnchor: String?

A localized message providing “help” text if the user requests help.

var rawValue: String

The corresponding value of the raw type.

var recoverySuggestion: String?

A localized message describing how one might recover from the failure.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

Error Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Error
- Hashable
- LocalizedError
- RawRepresentable
- Sendable

## See Also

### Token management

typealias MusicTokenProvider

An object that music requests use to access Apple Music API.

protocol MusicDeveloperTokenProvider

A set of methods that music requests use to access Apple Music API.

class MusicUserTokenProvider

A class that music requests use to fetch user tokens your app requires to access Apple Music API.

struct MusicTokenRequestOptions

Options that music requests pass into token provider methods to fetch a required token for accessing Apple Music API.

class DefaultMusicTokenProvider

The default token provider that music requests use to access Apple Music API.

