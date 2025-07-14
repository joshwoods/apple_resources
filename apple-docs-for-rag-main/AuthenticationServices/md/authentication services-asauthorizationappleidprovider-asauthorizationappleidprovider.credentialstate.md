

- Authentication Services
- ASAuthorizationAppleIDProvider
-  ASAuthorizationAppleIDProvider.CredentialState 

Enumeration

# ASAuthorizationAppleIDProvider.CredentialState

Possible values for the credential state of a user.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum CredentialState
```

## Topics

### User Credential States

case authorized

The user is authorized.

case notFound

The user hasn’t established a relationship with Sign in with Apple.

case revoked

The given user’s authorization has been revoked and they should be signed out.

case transferred

The app has been transferred to a different team, and you need to migrate the user’s identifier.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting State

func getCredentialState(forUserID: String, completion: (ASAuthorizationAppleIDProvider.CredentialState, (any Error)?) -> Void)

Returns the credential state for the given user in a completion handler.

class let credentialRevokedNotification: NSNotification.Name

A notification that indicates the user’s credentials have been revoked and they should be signed out.

