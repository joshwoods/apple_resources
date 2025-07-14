

- Authentication Services
-  ASAuthorizationWebBrowserPlatformPublicKeyCredentialAssertionRequest 

Protocol

# ASAuthorizationWebBrowserPlatformPublicKeyCredentialAssertionRequest

An interface you use to respond to authentication challenges in a web browser.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.6+macOS 13.5+

``` source
protocol ASAuthorizationWebBrowserPlatformPublicKeyCredentialAssertionRequest
```

## Topics

### Information about the assertion

var clientData: ASPublicKeyCredentialClientData?

The client data to supply to the relying party.

var shouldShowHybridTransport: Bool

Whether a remote authenticator that communicates with the operating system using Bluetooth can resolve the challenge.

**Required**

## Relationships

### Conforming Types

- ASAuthorizationPlatformPublicKeyCredentialAssertionRequest

## See Also

### Website authentication requests

protocol ASAuthorizationWebBrowserExternallyAuthenticatableRequest

An authorization request for which a web browser can retrieve credentials.

protocol ASAuthorizationWebBrowserPlatformPublicKeyCredentialRegistrationRequest

An interface you use to respond to passkey-creation challenges in a web browser.

