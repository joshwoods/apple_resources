

- Authentication Services
- ASPasskeyCredentialIdentity
-  credentialID 

Instance Property

# credentialID

The credential identifier for this passkey credential identity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var credentialID: Data { get }
```

## Discussion

Use the credential identifier, along with the userHandle, to identify the correct credential to use for a given relying party request.

## See Also

### Distinguishing identities

var recordIdentifier: String?

A string used to correlate this identity to a record in your app’s own database.

