

- Authentication Services
- ASAuthorizationWebBrowserPlatformPublicKeyCredentialProvider
-  createCredentialRegistrationRequest(clientData:name:userID:) 

Instance Method

# createCredentialRegistrationRequest(clientData:name:userID:)

Create a credential registration request, for registering a new passkey with the relying party.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.6+macOS 13.5+

``` source
func createCredentialRegistrationRequest(
    clientData: ASPublicKeyCredentialClientData,
    name: String,
    userID: Data
) -> ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest
```

**Required**

## Parameters 

`clientData`  

The client data that contains the reply to the relying party’s challenge.

`name`  

The person’s user name for their account with the relying party.

`userID`  

A unique identifier for the person’s account with the relying party.

## Return Value

The credential registration request, that you pass to ASAuthorizationController.

## See Also

### Creating requests

func createCredentialAssertionRequest(clientData: ASPublicKeyCredentialClientData) -> ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

Create a credential assertion request, for authenticating to the relying party.

**Required**

