

- Authentication Services
- ASAuthorizationSecurityKeyPublicKeyCredentialProvider
-  createCredentialAssertionRequest(challenge:) 

Instance Method

# createCredentialAssertionRequest(challenge:)

Creates an assertion request with a challenge.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func createCredentialAssertionRequest(challenge: Data) -> ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest
```

## Parameters 

`challenge`  

A stream of bytes that the server provides to prove an authenticator is valid.

## Return Value

A security key credential registration request.

## See Also

### Creating the request

var relyingPartyIdentifier: String

The domain name of the service to authorize against.

func createCredentialRegistrationRequest(challenge: Data, displayName: String, name: String, userID: Data) -> ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest

Creates an assertion request with a challenge, display name, and user ID.

