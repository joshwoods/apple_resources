

- RoomPlan
- CapturedRoom
- CapturedRoom.Object
-  confidence 

Instance Property

# confidence

A level of certainty in the object’s category.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var confidence: CapturedRoom.Confidence { get }
```

## See Also

### Identifying an object

var identifier: UUID

A unique alphanumeric value that the framework assigns the object.

var parentIdentifier: UUID?

A unique alphanumeric value that identifies the object’s parent object or surface.

var category: CapturedRoom.Object.Category

A classification that the captured room assigns the object.

enum Category

Classifications of an object in a captured room.

