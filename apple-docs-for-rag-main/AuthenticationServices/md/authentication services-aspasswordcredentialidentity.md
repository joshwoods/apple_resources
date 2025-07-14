

- Authentication Services
-  ASPasswordCredentialIdentity 

Class

# ASPasswordCredentialIdentity

A description that uniquely identifies a particular password credential.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class ASPasswordCredentialIdentity
```

## Topics

### Creating a credential identity

init(serviceIdentifier: ASCredentialServiceIdentifier, user: String, recordIdentifier: String?)

Initializes a password credential identity.

class ASCredentialServiceIdentifier

An identifier representing a particular service for which the user needs a credential, like a web site.

### Ordering credential identities

var rank: Int

An indicator that enables you to prioritze credential identities relative to each other.

### Associating a user

var user: String

The username associated with the credential.

### Distinguishing identities

var recordIdentifier: String?

A string used to correlate this identity to a record in your app’s own database.

var serviceIdentifier: ASCredentialServiceIdentifier

An identifier that helps the system know with which apps or websites to associate this credential.

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

class ASPasskeyCredentialIdentity

A description that uniquely identifies a particular passkey credential.

