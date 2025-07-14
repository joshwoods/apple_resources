

- Authentication Services
- ASPasskeyAssertionCredential
-  userHandle 

Instance Property

# userHandle

The user handle of this passkey.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var userHandle: Data { get }
```

## See Also

### Accessing credential information

var authenticatorData: Data

The authenticator data of the application that created this passkey assertion credential.

var clientDataHash: Data

A hash of the client data for this credential.

var credentialID: Data

The identifier for this credential.

var relyingParty: String

The relying party associated with this passkey.

var signature: Data

The cryptographic signature of this credential.

