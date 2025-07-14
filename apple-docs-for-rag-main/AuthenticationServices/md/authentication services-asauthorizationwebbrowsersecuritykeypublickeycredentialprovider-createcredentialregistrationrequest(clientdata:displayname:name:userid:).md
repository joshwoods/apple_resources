

- Authentication Services
- ASAuthorizationWebBrowserSecurityKeyPublicKeyCredentialProvider
-  createCredentialRegistrationRequest(clientData:displayName:name:userID:) 

Instance Method

# createCredentialRegistrationRequest(clientData:displayName:name:userID:)

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+

``` source
func createCredentialRegistrationRequest(
    clientData: ASPublicKeyCredentialClientData,
    displayName: String,
    name: String,
    userID: Data
) -> ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest
```

**Required**

## See Also

### Creating passkey assertion requests

func createCredentialAssertionRequest(clientData: ASPublicKeyCredentialClientData) -> ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

**Required**

