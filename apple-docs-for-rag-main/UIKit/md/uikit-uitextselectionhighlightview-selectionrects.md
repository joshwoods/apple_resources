

- UIKit
- UITextSelectionHighlightView
-  selectionRects 

Instance Property

# selectionRects

The rectangles to draw with the selection highlight.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var selectionRects: [UITextSelectionRect] { get set }
```

**Required**

## Discussion

Use this property to get the rectangles to draw in a custom highlight view. The rectangles are in the coordinate space of the view that adopts this protocol.

