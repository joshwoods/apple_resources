

- RoomPlan
- CapturedRoom
- CapturedRoom.Object
-  attributes 

Instance Property

# attributes

A collection of details that describe a particular object in the room.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var attributes: [any CapturedRoomAttribute] { get }
```

## See Also

### Describing an object

func attribute&lt;T>(of: T.Type) -> T?

Checks an object for specific attribute types.

