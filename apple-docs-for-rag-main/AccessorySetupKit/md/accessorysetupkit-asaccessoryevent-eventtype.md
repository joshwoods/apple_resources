

- AccessorySetupKit
- ASAccessoryEvent
-  eventType 

Instance Property

# eventType

The type of event, such as accessory addition or removal, or picker presentation or removal.

iOS 18.0+iPadOS 18.0+

``` source
var eventType: ASAccessoryEventType { get }
```

## Mentioned in 

Discovering and configuring accessories

## Discussion

Some event types may indicate that the event is a subclass of ASAccessoryEvent that provides additional properties.

## See Also

### Inspecting the event

var accessory: ASAccessory?

The accessory involved in the event, if any.

class ASAccessory

An accessory discovered by the accessory session.

enum ASAccessoryEventType

An enumeration of the types of events encountered during accessory discovery

