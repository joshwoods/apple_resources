

- UIKit
- UITextDragPreviewRenderer
-  init(layoutManager:range:unifyRects:) 

Initializer

# init(layoutManager:range:unifyRects:)

Returns an initialized renderer of a text drag preview with the specified layout manager, range, and rectangle detection behavior.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(
    layoutManager: NSLayoutManager,
    range: NSRange,
    unifyRects: Bool
)
```

## Parameters 

`layoutManager`  

The layout manager that renders the preview.

`range`  

The range to render the preview.

`unifyRects`  

A Boolean value that indicates whether the vertical position and height of the detection rectangles adjust to touch each other. If `true`, the firstLineRect, bodyRect, and lastLineRect properties adjust; otherwise, they don’t. The default value is `true`.

## Return Value

A renderer of a text drag preview using the specified layout manager, range, and detection behavior.

## See Also

### Initializing a text drag preview renderer

convenience init(layoutManager: NSLayoutManager, range: NSRange)

Initializes and returns a text drag preview renderer with the specified layout managers and range to render the text drag preview.

