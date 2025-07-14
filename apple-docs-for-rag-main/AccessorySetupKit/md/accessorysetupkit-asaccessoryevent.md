

- AccessorySetupKit
-  ASAccessoryEvent 

Class

# ASAccessoryEvent

Properties of an event encountered during accessory discovery.

iOS 18.0+iPadOS 18.0+

``` source
class ASAccessoryEvent
```

## Mentioned in 

Discovering and configuring accessories

## Overview

The event handler you register with the session’s activate(on:eventHandler:) method receives objects of this type from the session. Each event identifies the type of event and which accessory (if any) is involved.

## Topics

### Inspecting the event

var accessory: ASAccessory?

The accessory involved in the event, if any.

class ASAccessory

An accessory discovered by the accessory session.

var eventType: ASAccessoryEventType

The type of event, such as accessory addition or removal, or picker presentation or removal.

enum ASAccessoryEventType

An enumeration of the types of events encountered during accessory discovery

### Handling errors

var error: (any Error)?

The error associated with the event, if any.

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
- Sendable

## See Also

### Accessory discovery

enum ASAccessoryEventType

An enumeration of the types of events encountered during accessory discovery

class ASDiscoveryDescriptor

Descriptive traits used to discover accessories.

