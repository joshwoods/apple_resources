

- Authentication Services
- ASAuthorizationAppleIDProvider
-  credentialRevokedNotification 

Type Property

# credentialRevokedNotification

A notification that indicates the user’s credentials have been revoked and they should be signed out.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class let credentialRevokedNotification: NSNotification.Name
```

## See Also

### Getting State

func getCredentialState(forUserID: String, completion: (ASAuthorizationAppleIDProvider.CredentialState, (any Error)?) -> Void)

Returns the credential state for the given user in a completion handler.

enum CredentialState

Possible values for the credential state of a user.

