

- RoomPlan
- CapturedRoom
- CapturedRoom.Surface
-  parentIdentifier 

Instance Property

# parentIdentifier

A unique alphanumeric value that identifies a surface’s parent surface.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var parentIdentifier: UUID? { get }
```

## Discussion

For example, the parent of a window is the wall surface on which the window rests.

## See Also

### Identifying a surface

var identifier: UUID

A unique alphanumeric value that the framework assigns the surface.

var category: CapturedRoom.Surface.Category

A classification that the captured room assigns the surface.

enum Category

Classifications of a surface in a captured room.

var confidence: CapturedRoom.Confidence

A level of certainty in the surface’s category.

