

- Authentication Services
-  ASCredentialIdentityStore 

Class

# ASCredentialIdentityStore

A container that your extension fills to provide credentials through the QuickType bar.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class ASCredentialIdentityStore
```

## Overview

Make credential identities available to users directly as AutoFill suggestions by adding them to the shared instance of the identity store. You can add identities during configuration in your extension’s override of the prepareInterfaceForExtensionConfiguration() method. You can also update the shared store from within your extension’s host app.

Be sure to update the shared store whenever your app’s database changes to avoid showing stale identities as AutoFill suggestions. Take advantage of the incremental change methods saveCredentialIdentities(_:completion:) and removeCredentialIdentities(_:completion:) to avoid rewriting the entire store every time you need to make a change.

When the user disables your extension, the system clears and disables your shared store. So before making updates, check to see that the store’s enabled to avoid unnecessary activity:

- Swift
- Objective-C

```
let store = ASCredentialIdentityStore.shared
store.getState { state in
    if state.isEnabled {
        // Add, remove, or update identities.
    }
}
```

```
```

## Topics

### Getting the shared store

class var shared: ASCredentialIdentityStore

The shared credential identity store.

### Checking the state of the store

func getState((ASCredentialIdentityStoreState) -> Void)

Gets the state of the credential identity store.

class ASCredentialIdentityStoreState

A representation of the state of a credential identity store.

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

class ASPasswordCredentialIdentity

A description that uniquely identifies a particular password credential.

### Recognizing errors

struct ASCredentialIdentityStoreError

A credential identity store error.

let ASCredentialIdentityStoreErrorDomain: String

The domain for a credential identity store error.

enum Code

Constants that represent credential identity store error codes.

### Deprecated methods

func saveCredentialIdentities([ASPasswordCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Saves the given credential identities to the store.

Deprecated

func replaceCredentialIdentities(with: [ASPasswordCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Replaces existing credential identities with new credential identities.

Deprecated

func removeCredentialIdentities([ASPasswordCredentialIdentity], completion: ((Bool, (any Error)?) -> Void)?)

Removes the given credential identities from the store.

Deprecated

### Instance Methods

func credentialIdentities(forService: ASCredentialServiceIdentifier?, credentialIdentityTypes: ASCredentialIdentityStore.IdentityTypes) async -> [any ASCredentialIdentity]

### Structures

struct IdentityTypes

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Configuring the credential provider extension

func prepareInterfaceForExtensionConfiguration()

Prepares the interface to enable the user to configure the extension.

