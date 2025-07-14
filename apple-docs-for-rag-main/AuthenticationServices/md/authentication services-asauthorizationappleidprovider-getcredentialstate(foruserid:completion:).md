

- Authentication Services
- ASAuthorizationAppleIDProvider
-  getCredentialState(forUserID:completion:) 

Instance Method

# getCredentialState(forUserID:completion:)

Returns the credential state for the given user in a completion handler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func getCredentialState(
    forUserID userID: String,
    completion: @escaping (ASAuthorizationAppleIDProvider.CredentialState, (any Error)?) -> Void
)
```

``` source
func credentialState(forUserID userID: String) async throws -> ASAuthorizationAppleIDProvider.CredentialState
```

## Parameters 

`userID`  

An opaque string associated with the Apple ID that your app receives in the credential’s user property after performing a successful authentication request.

`completion`  

A block the method calls to report the state and an optional error condition.

## See Also

### Getting State

enum CredentialState

Possible values for the credential state of a user.

class let credentialRevokedNotification: NSNotification.Name

A notification that indicates the user’s credentials have been revoked and they should be signed out.

