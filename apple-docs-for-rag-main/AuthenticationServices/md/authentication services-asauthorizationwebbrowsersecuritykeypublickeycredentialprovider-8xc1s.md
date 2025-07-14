

- Authentication Services
-  ASAuthorizationWebBrowserSecurityKeyPublicKeyCredentialProvider 

Protocol

# ASAuthorizationWebBrowserSecurityKeyPublicKeyCredentialProvider

A protocol for creating passkey requests.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+

``` source
protocol ASAuthorizationWebBrowserSecurityKeyPublicKeyCredentialProvider
```

## Topics

### Creating passkey assertion requests

func createCredentialAssertionRequest(clientData: ASPublicKeyCredentialClientData) -> ASAuthorizationSecurityKeyPublicKeyCredentialAssertionRequest

**Required**

func createCredentialRegistrationRequest(clientData: ASPublicKeyCredentialClientData, displayName: String, name: String, userID: Data) -> ASAuthorizationSecurityKeyPublicKeyCredentialRegistrationRequest

**Required**

## Relationships

### Conforming Types

- ASAuthorizationSecurityKeyPublicKeyCredentialProvider

