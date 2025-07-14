

- Authentication Services
- ASAuthorizationPlatformPublicKeyCredentialProvider
-  createCredentialRegistrationRequest(challenge:name:userID:) 

Instance Method

# createCredentialRegistrationRequest(challenge:name:userID:)

Creates an assertion request with a challenge, name, and user ID.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
func createCredentialRegistrationRequest(
    challenge: Data,
    name: String,
    userID: Data
) -> ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest
```

## Parameters 

`challenge`  

A stream of bytes that the server provides to prove an authenticator is valid.

`name`  

The name of the user.

`userID`  

A user identifier.

## Return Value

A public key credential registration request.

## See Also

### Creating the request

var relyingPartyIdentifier: String

The domain name of the service to register or authorize against.

func createCredentialAssertionRequest(challenge: Data) -> ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

Creates an assertion request with a challenge.

