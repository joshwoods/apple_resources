

- Authentication Services
- ASAuthorizationPlatformPublicKeyCredentialProvider
-  relyingPartyIdentifier 

Instance Property

# relyingPartyIdentifier

The domain name of the service to register or authorize against.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var relyingPartyIdentifier: String { get }
```

## See Also

### Creating the request

func createCredentialAssertionRequest(challenge: Data) -> ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

Creates an assertion request with a challenge.

func createCredentialRegistrationRequest(challenge: Data, name: String, userID: Data) -> ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

Creates an assertion request with a challenge, name, and user ID.

