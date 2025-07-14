

- Authentication Services
- ASAuthorizationPlatformPublicKeyCredentialProvider
-  createCredentialAssertionRequest(challenge:) 

Instance Method

# createCredentialAssertionRequest(challenge:)

Creates an assertion request with a challenge.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func createCredentialAssertionRequest(challenge: Data) -> ASAuthorizationPlatformPublicKeyCredentialAssertionRequest
```

## Parameters 

`challenge`  

A stream of bytes that the server provides to prove an authenticator is valid.

## Return Value

A public key credential registration request.

## See Also

### Creating the request

var relyingPartyIdentifier: String

The domain name of the service to register or authorize against.

func createCredentialRegistrationRequest(challenge: Data, name: String, userID: Data) -> ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

Creates an assertion request with a challenge, name, and user ID.

