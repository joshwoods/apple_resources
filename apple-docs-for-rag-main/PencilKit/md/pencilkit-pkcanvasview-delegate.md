

- PencilKit
- PKCanvasView
-  delegate 

Instance Property

# delegate

The object you use to respond to changes in the drawn content or with the selected tool.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any PKCanvasViewDelegate)? { get set }
```

## See Also

### Responding to drawing-related changes

protocol PKCanvasViewDelegate

Methods for monitoring drawing related changes in a canvas view.

