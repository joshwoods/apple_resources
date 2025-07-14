

- UIKit
- UIEvent
-  subtype 

Instance Property

# subtype

Returns the subtype of the event.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var subtype: UIEvent.EventSubtype { get }
```

## Discussion

The UIEvent.EventSubtype constant returned by this property indicates the subtype of the event in relation to the general type, which you can retrieve from the type property.

## See Also

### Getting the event type

var type: UIEvent.EventType

Returns the type of the event.

enum EventType

Constants that specify the general type of an event.

enum EventSubtype

Constants that specify the subtype of the event in relation to its general type.

