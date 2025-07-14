

- AccessorySetupKit
- ASAccessoryEvent
-  accessory 

Instance Property

# accessory

The accessory involved in the event, if any.

iOS 18.0+iPadOS 18.0+

``` source
@NSCopying
var accessory: ASAccessory? { get }
```

## Mentioned in 

Discovering and configuring accessories

## Discussion

The session populates this member for event types like ASAccessoryEventType.accessoryAdded and ASAccessoryEventType.accessoryChanged, but not for life cycle or picker events like ASAccessoryEventType.activated or ASAccessoryEventType.pickerDidPresent.

## See Also

### Inspecting the event

class ASAccessory

An accessory discovered by the accessory session.

var eventType: ASAccessoryEventType

The type of event, such as accessory addition or removal, or picker presentation or removal.

enum ASAccessoryEventType

An enumeration of the types of events encountered during accessory discovery

