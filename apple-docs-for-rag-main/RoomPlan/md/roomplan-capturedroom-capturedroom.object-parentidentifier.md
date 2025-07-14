

- RoomPlan
- CapturedRoom
- CapturedRoom.Object
-  parentIdentifier 

Instance Property

# parentIdentifier

A unique alphanumeric value that identifies the object’s parent object or surface.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var parentIdentifier: UUID? { get }
```

## Discussion

For example, the parent of a sink is the storage area in which the sink resides.

## See Also

### Identifying an object

var identifier: UUID

A unique alphanumeric value that the framework assigns the object.

var category: CapturedRoom.Object.Category

A classification that the captured room assigns the object.

enum Category

Classifications of an object in a captured room.

var confidence: CapturedRoom.Confidence

A level of certainty in the object’s category.

