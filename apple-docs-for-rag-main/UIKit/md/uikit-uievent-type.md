

- UIKit
- UIEvent
-  type 

Instance Property

# type

Returns the type of the event.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var type: UIEvent.EventType { get }
```

## Discussion

The UIEvent.EventType constant returned by this property indicates the general type of this event — for example, whether it’s a touch or motion event.

## See Also

### Getting the event type

enum EventType

Constants that specify the general type of an event.

var subtype: UIEvent.EventSubtype

Returns the subtype of the event.

enum EventSubtype

Constants that specify the subtype of the event in relation to its general type.

