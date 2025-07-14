

- RoomPlan
- CapturedRoom
- CapturedRoom.Object
-  identifier 

Instance Property

# identifier

A unique alphanumeric value that the framework assigns the object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var identifier: UUID { get }
```

## See Also

### Identifying an object

var parentIdentifier: UUID?

A unique alphanumeric value that identifies the object’s parent object or surface.

var category: CapturedRoom.Object.Category

A classification that the captured room assigns the object.

enum Category

Classifications of an object in a captured room.

var confidence: CapturedRoom.Confidence

A level of certainty in the object’s category.

