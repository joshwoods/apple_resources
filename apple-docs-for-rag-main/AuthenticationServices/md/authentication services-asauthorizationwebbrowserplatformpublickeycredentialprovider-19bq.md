

- Authentication Services
-  ASAuthorizationWebBrowserPlatformPublicKeyCredentialProvider 

Protocol

# ASAuthorizationWebBrowserPlatformPublicKeyCredentialProvider

A mechanism you use to provide public key credential requests to a browser app.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.6+macOS 13.5+

``` source
protocol ASAuthorizationWebBrowserPlatformPublicKeyCredentialProvider
```

## Topics

### Creating requests

func createCredentialAssertionRequest(clientData: ASPublicKeyCredentialClientData) -> ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

Create a credential assertion request, for authenticating to the relying party.

**Required**

func createCredentialRegistrationRequest(clientData: ASPublicKeyCredentialClientData, name: String, userID: Data) -> ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

Create a credential registration request, for registering a new passkey with the relying party.

**Required**

### Instance Methods

func createCredentialRegistrationRequest(clientData: ASPublicKeyCredentialClientData, name: String, userID: Data, requestStyle: ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest.RequestStyle) -> ASAuthorizationPlatformPublicKeyCredentialRegistrationRequest

**Required**

## Relationships

### Conforming Types

- ASAuthorizationPlatformPublicKeyCredentialProvider

