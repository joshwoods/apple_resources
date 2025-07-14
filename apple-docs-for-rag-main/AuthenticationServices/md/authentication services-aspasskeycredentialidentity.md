

- Authentication Services
-  ASPasskeyCredentialIdentity 

Class

# ASPasskeyCredentialIdentity

A description that uniquely identifies a particular passkey credential.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
class ASPasskeyCredentialIdentity
```

## Topics

### Creating a credential identity

convenience init(relyingPartyIdentifier: String, userName: String, credentialID: Data, userHandle: Data, recordIdentifier: String?)

Initializes a passkey credential identity.

convenience init(relyingPartyIdentifier: String, userName: String, credentialID: Data, userHandle: Data, recordIdentifier: String?)

Creates and initializes a passkey credential identity.

### Ordering credential identities

var rank: Int

An indicator that enables you to prioritize credential identities relative to each other.

### Associating a user

var userName: String

The username of this passkey credential.

var userHandle: Data

The user handle of this passkey credential.

### Associating a relying party

var relyingPartyIdentifier: String

A string that identifies this identity’s relying party.

### Distinguishing identities

var credentialID: Data

The credential identifier for this passkey credential identity.

var recordIdentifier: String?

A string used to correlate this identity to a record in your app’s own database.

## Relationships

### Inherits From

- NSObject

### Conforms To

- ASCredentialIdentity
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Adding and removing credential identities

func saveCredentialIdentities([any ASCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Save the supplied credential identities to the store.

func replaceCredentialIdentities([any ASCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Replaces existing credential identities with new credential identities.

func removeAllCredentialIdentities(((Bool, (any Error)?) -> Void)?)

Removes all existing credential identities from the store.

func removeCredentialIdentities([any ASCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Remove the given credential identities from the store.

protocol ASCredentialIdentity

A protocol that credential identity classes conform to that uniquely identifies credentials.

class ASPasswordCredentialIdentity

A description that uniquely identifies a particular password credential.

