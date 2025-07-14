

- Authentication Services
- ASAuthorizationWebBrowserPlatformPublicKeyCredentialRegistrationRequest
-  excludedCredentials 

Instance Property

# excludedCredentials

A list of passkeys that the relying party doesn’t accept for resolving the challenge.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.6+macOS 13.5+

``` source
var excludedCredentials: [ASAuthorizationPlatformPublicKeyCredentialDescriptor]? { get set }
```

**Required**

## See Also

### Information about the assertion

var clientData: ASPublicKeyCredentialClientData?

The client data to supply to the relying party.

var shouldShowHybridTransport: Bool

Whether a remote authenticator that communicates with the operating system using Bluetooth can resolve the challenge.

**Required**

