

- Authentication Services
- ASAuthorizationSecurityKeyPublicKeyCredentialProvider
-  createCredentialRegistrationRequest(challenge:displayName:name:userID:) 

Instance Method

# createCredentialRegistrationRequest(challenge:displayName:name:userID:)

Creates an assertion request with a challenge, display name, and user ID.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
func createCredentialRegistrationRequest(
    challenge: Data,
    displayName: String,
    name: String,
    userID: Data
) -> ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest
```

## Parameters 

`challenge`  

A stream of bytes that the server provides to prove an authenticator is valid.

`displayName`  

The proper name of the user.

`name`  

The name of the user.

`userID`  

The user’s account identifier.

## Return Value

A security key credential registration request.

## Mentioned in 

Supporting Security Key Authentication Using Physical Keys

Supporting passkeys

## See Also

### Creating the request

var relyingPartyIdentifier: String

The domain name of the service to authorize against.

func createCredentialAssertionRequest(challenge: Data) -> ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

Creates an assertion request with a challenge.

