

- Authentication Services
-  ASCredentialIdentityStoreState 

Class

# ASCredentialIdentityStoreState

A representation of the state of a credential identity store.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class ASCredentialIdentityStoreState
```

## Topics

### Checking the state

var isEnabled: Bool

A Boolean value indicating whether the credential identity store is enabled.

var supportsIncrementalUpdates: Bool

A Boolean value indicating whether the credential identity store supports incremental updates.

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

### Checking the state of the store

func getState((ASCredentialIdentityStoreState) -> Void)

Gets the state of the credential identity store.

