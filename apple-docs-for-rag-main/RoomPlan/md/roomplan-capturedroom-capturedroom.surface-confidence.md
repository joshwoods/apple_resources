

- RoomPlan
- CapturedRoom
- CapturedRoom.Surface
-  confidence 

Instance Property

# confidence

A level of certainty in the surface’s category.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var confidence: CapturedRoom.Confidence { get }
```

## See Also

### Identifying a surface

var identifier: UUID

A unique alphanumeric value that the framework assigns the surface.

var parentIdentifier: UUID?

A unique alphanumeric value that identifies a surface’s parent surface.

var category: CapturedRoom.Surface.Category

A classification that the captured room assigns the surface.

enum Category

Classifications of a surface in a captured room.

