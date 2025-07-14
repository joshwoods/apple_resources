

- RoomPlan
- CapturedRoom
- CapturedRoom.Surface
-  category 

Instance Property

# category

A classification that the captured room assigns the surface.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var category: CapturedRoom.Surface.Category { get }
```

## See Also

### Identifying a surface

var identifier: UUID

A unique alphanumeric value that the framework assigns the surface.

var parentIdentifier: UUID?

A unique alphanumeric value that identifies a surface’s parent surface.

enum Category

Classifications of a surface in a captured room.

var confidence: CapturedRoom.Confidence

A level of certainty in the surface’s category.

