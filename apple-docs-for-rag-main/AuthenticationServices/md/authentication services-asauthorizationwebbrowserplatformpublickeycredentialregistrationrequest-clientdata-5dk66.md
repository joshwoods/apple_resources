

- Authentication Services
- ASAuthorizationWebBrowserPlatformPublicKeyCredentialRegistrationRequest
-  clientData 

Instance Property

# clientData

The client data to supply to the relying party.

Mac Catalyst 16.6+macOS 13.5+

``` source
var clientData: ASPublicKeyCredentialClientData? { get }
```

## See Also

### Information about the assertion

var excludedCredentials: [ASAuthorizationPlatformPublicKeyCredentialDescriptor]?

A list of passkeys that the relying party doesn’t accept for resolving the challenge.

**Required**

var shouldShowHybridTransport: Bool

Whether a remote authenticator that communicates with the operating system using Bluetooth can resolve the challenge.

**Required**

