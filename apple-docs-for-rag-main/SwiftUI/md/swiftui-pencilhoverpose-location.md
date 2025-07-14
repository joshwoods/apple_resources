

- SwiftUI
- PencilHoverPose
-  location 

Instance Property

# location

The location of an Apple Pencil hovering in the area above the view’s bounds, expressed as a point in that view’s coordinate space.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+macOS 14.5+

``` source
let location: CGPoint
```

## Discussion

Use the anchor property if you require a normalized anchor point for use with a presentation modifier instead.

## See Also

### Getting the hover characteristics

let anchor: UnitPoint

The location of an Apple Pencil hovering in the area above the view’s bounds, expressed as a normalized anchor point relative to that view.

let zDistance: CGFloat

The normalized distance between the screen and a hovering Apple Pencil.

