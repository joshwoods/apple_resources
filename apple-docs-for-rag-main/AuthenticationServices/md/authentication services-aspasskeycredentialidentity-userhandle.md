

- Authentication Services
- ASPasskeyCredentialIdentity
-  userHandle 

Instance Property

# userHandle

The user handle of this passkey credential.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var userHandle: Data { get }
```

## Discussion

Use the user handle, along with the credentialID, to identify the correct credential to use for a given relying party request.

## See Also

### Associating a user

var userName: String

The username of this passkey credential.

