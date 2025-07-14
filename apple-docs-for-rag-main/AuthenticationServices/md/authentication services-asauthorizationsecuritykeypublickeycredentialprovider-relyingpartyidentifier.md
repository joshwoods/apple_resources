

- Authentication Services
- ASAuthorizationSecurityKeyPublicKeyCredentialProvider
-  relyingPartyIdentifier 

Instance Property

# relyingPartyIdentifier

The domain name of the service to authorize against.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var relyingPartyIdentifier: String { get }
```

## See Also

### Creating the request

func createCredentialAssertionRequest(challenge: Data) -> ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

Creates an assertion request with a challenge.

func createCredentialRegistrationRequest(challenge: Data, displayName: String, name: String, userID: Data) -> ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest

Creates an assertion request with a challenge, display name, and user ID.

