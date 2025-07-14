

- AccessorySetupKit
- ASAccessory
-  ASAccessory.AccessoryState 

Enumeration

# ASAccessory.AccessoryState

An enumeration of possible authorization states of an accessory.

iOS 18.0+iPadOS 18.0+

``` source
enum AccessoryState
```

## Topics

### Creating a state instance

init?(rawValue: Int)

### Accessory states

case authorized

case awaitingAuthorization

case unauthorized

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessory description

class ASAccessory

An accessory discovered by the accessory session.

