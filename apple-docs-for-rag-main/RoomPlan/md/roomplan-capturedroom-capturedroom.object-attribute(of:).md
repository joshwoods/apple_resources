

- RoomPlan
- CapturedRoom
- CapturedRoom.Object
-  attribute(of:) 

Instance Method

# attribute(of:)

Checks an object for specific attribute types.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
func attribute(of attributeType: T.Type) -> T? where T : CapturedRoomAttribute
```

## Discussion

This function provides details about an object based on attribute type. For example, the following code checks whether an object the framework observes during a scan resembles a dining table:

```
```

## See Also

### Describing an object

var attributes: [any CapturedRoomAttribute]

A collection of details that describe a particular object in the room.

