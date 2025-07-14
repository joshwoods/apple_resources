

- SwiftUI
- PencilHoverPose
-  anchor 

Instance Property

# anchor

The location of an Apple Pencil hovering in the area above the view’s bounds, expressed as a normalized anchor point relative to that view.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+macOS 14.5+

``` source
let anchor: UnitPoint
```

## Discussion

You can pass this anchor point directly to a presentation modifier like popover(isPresented:attachmentAnchor:arrowEdge:content:) or use the location property if you require an absolute point instead.

## See Also

### Getting the hover characteristics

let location: CGPoint

The location of an Apple Pencil hovering in the area above the view’s bounds, expressed as a point in that view’s coordinate space.

let zDistance: CGFloat

The normalized distance between the screen and a hovering Apple Pencil.

