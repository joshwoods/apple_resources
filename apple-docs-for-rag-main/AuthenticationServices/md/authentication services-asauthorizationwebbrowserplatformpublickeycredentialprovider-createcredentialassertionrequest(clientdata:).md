

- Authentication Services
- ASAuthorizationWebBrowserPlatformPublicKeyCredentialProvider
-  createCredentialAssertionRequest(clientData:) 

Instance Method

# createCredentialAssertionRequest(clientData:)

Create a credential assertion request, for authenticating to the relying party.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.6+macOS 13.5+

``` source
func createCredentialAssertionRequest(clientData: ASPublicKeyCredentialClientData) -> ASAuthorizationPlatformPublicKeyCredentialAssertionRequest
```

**Required**

## Parameters 

`clientData`  

The client data that contains the reply to the relying party’s challenge.

## Return Value

The credential assertion request, that you pass to ASAuthorizationController.

## See Also

### Creating requests

func createCredentialRegistrationRequest(clientData: ASPublicKeyCredentialClientData, name: String, userID: Data) -> ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

Create a credential registration request, for registering a new passkey with the relying party.

**Required**

