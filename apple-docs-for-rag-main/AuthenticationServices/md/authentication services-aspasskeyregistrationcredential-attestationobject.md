

- Authentication Services
- ASPasskeyRegistrationCredential
-  attestationObject 

Instance Property

# attestationObject

The attestation object for this passkey.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var attestationObject: Data { get }
```

## Discussion

The relying party may use information in the attestation object to assess the origin of a passkey during registration.

## See Also

### Accessing credential information

var clientDataHash: Data

A hash of the client data for this credential.

var credentialID: Data

The identifier for this credential.

var relyingParty: String

The relying party associated with this passkey.

