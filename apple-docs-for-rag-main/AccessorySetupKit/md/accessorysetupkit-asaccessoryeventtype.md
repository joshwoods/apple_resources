

- AccessorySetupKit
-  ASAccessoryEventType 

Enumeration

# ASAccessoryEventType

An enumeration of the types of events encountered during accessory discovery

iOS 18.0+iPadOS 18.0+Mac Catalyst

``` source
enum ASAccessoryEventType
```

## Topics

### Creating an event type instance

init?(rawValue: Int)

### Accessory events

case accessoryAdded

The session added an accessory.

case accessoryChanged

The properties of an accessory changed.

case accessoryRemoved

The session removed an accessory.

### Life cycle events

case activated

The discovery session activated.

case invalidated

The discovery session invalidated.

### Picker events

case pickerDidPresent

The discovery session picker appeared.

case pickerDidDismiss

The discovery session picker dismissed.

case pickerSetupBridging

The discovery session picker started bridging with an accessory.

case pickerSetupPairing

The discovery session picker started pairing with a Bluetooth accessory.

case pickerSetupFailed

The discovery session picker setup failed.

case pickerSetupRename

The discovery session picker started renaming an accessory.

### Migration events

case migrationComplete

The migration of an accessory completed.

### Unclassified events

case unknown

An unknown event occurred.

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

### Accessory discovery

class ASAccessoryEvent

Properties of an event encountered during accessory discovery.

class ASDiscoveryDescriptor

Descriptive traits used to discover accessories.

