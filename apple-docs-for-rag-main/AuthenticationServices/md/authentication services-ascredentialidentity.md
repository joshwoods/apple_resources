

- Authentication Services
-  ASCredentialIdentity 

Protocol

# ASCredentialIdentity

A protocol that credential identity classes conform to that uniquely identifies credentials.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
protocol ASCredentialIdentity : NSObjectProtocol
```

## Topics

### Ordering credential identities

var rank: Int

An indicator that enables you to prioritize credential identities relative to each other.

**Required**

### Associating a user

var user: String

The username associated with this credential.

**Required**

### Distinguishing identities

var recordIdentifier: String?

A string used to correlate this identity to a record in your app’s own database.

**Required**

var serviceIdentifier: ASCredentialServiceIdentifier

An identifier that helps the system know with which apps or websites to associate this credential.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- ASOneTimeCodeCredentialIdentity
- ASPasskeyCredentialIdentity
- ASPasswordCredentialIdentity

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

class ASPasskeyCredentialIdentity

A description that uniquely identifies a particular passkey credential.

class ASPasswordCredentialIdentity

A description that uniquely identifies a particular password credential.

