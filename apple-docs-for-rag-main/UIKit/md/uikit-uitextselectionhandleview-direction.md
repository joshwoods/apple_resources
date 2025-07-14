

- UIKit
- UITextSelectionHandleView
-  direction 

Instance Property

# direction

The orientation of the selection handle.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var direction: NSDirectionalRectEdge { get set }
```

**Required**

## Discussion

Specify leading if this view represents the leading selection handle or trailing if it represents the trailing selection handle. The system uses this information to determine where to differentiate the selection handles visually.

## See Also

### Specifying the handle details

var customShape: UIBezierPath?

The custom shape to draw for the stem of the selection handle.

**Required**

var isVertical: Bool

**Required**

