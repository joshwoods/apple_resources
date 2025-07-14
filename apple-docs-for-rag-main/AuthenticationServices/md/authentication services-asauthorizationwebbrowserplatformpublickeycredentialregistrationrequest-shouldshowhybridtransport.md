

- Authentication Services
- ASAuthorizationWebBrowserPlatformPublicKeyCredentialRegistrationRequest
-  shouldShowHybridTransport 

Instance Property

# shouldShowHybridTransport

Whether a remote authenticator that communicates with the operating system using Bluetooth can resolve the challenge.

Mac Catalyst 16.6+macOS 13.5+

``` source
var shouldShowHybridTransport: Bool { get set }
```

**Required**

## See Also

### Information about the assertion

var clientData: ASPublicKeyCredentialClientData?

The client data to supply to the relying party.

var excludedCredentials: [ASAuthorizationPlatformPublicKeyCredentialDescriptor]?

A list of passkeys that the relying party doesn’t accept for resolving the challenge.

**Required**

