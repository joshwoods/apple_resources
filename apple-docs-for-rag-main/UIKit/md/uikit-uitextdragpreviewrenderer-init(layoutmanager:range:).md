

- UIKit
- UITextDragPreviewRenderer
-  init(layoutManager:range:) 

Initializer

# init(layoutManager:range:)

Initializes and returns a text drag preview renderer with the specified layout managers and range to render the text drag preview.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
convenience init(
    layoutManager: NSLayoutManager,
    range: NSRange
)
```

## Parameters 

`layoutManager`  

The layout manager that renders the text drag preview.

`range`  

The range to render the text drag preview.

## Return Value

A renderer of a text drag preview using the specified layout manager and range.

## See Also

### Initializing a text drag preview renderer

init(layoutManager: NSLayoutManager, range: NSRange, unifyRects: Bool)

Returns an initialized renderer of a text drag preview with the specified layout manager, range, and rectangle detection behavior.

