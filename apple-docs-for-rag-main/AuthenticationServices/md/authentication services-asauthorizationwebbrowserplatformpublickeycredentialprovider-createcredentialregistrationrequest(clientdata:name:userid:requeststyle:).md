

- Authentication Services
- ASAuthorizationWebBrowserPlatformPublicKeyCredentialProvider
-  createCredentialRegistrationRequest(clientData:name:userID:requestStyle:) 

Instance Method

# createCredentialRegistrationRequest(clientData:name:userID:requestStyle:)

iOS 18.0+iPadOS 18.0+Mac Catalyst 16.6+macOS 15.0+

``` source
func createCredentialRegistrationRequest(
    clientData: ASPublicKeyCredentialClientData,
    name: String,
    userID: Data,
    requestStyle: ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest.RequestStyle
) -> ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest
```

**Required**

