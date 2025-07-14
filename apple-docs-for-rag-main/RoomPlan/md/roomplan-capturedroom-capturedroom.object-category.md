

- RoomPlan
- CapturedRoom
- CapturedRoom.Object
-  category 

Instance Property

# category

A classification that the captured room assigns the object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var category: CapturedRoom.Object.Category { get }
```

## See Also

### Identifying an object

var identifier: UUID

A unique alphanumeric value that the framework assigns the object.

var parentIdentifier: UUID?

A unique alphanumeric value that identifies the object’s parent object or surface.

enum Category

Classifications of an object in a captured room.

var confidence: CapturedRoom.Confidence

A level of certainty in the object’s category.

