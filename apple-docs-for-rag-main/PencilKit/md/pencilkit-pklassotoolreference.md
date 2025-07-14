

- PencilKit
-  PKLassoToolReference 

Class

# PKLassoToolReference

A tool for selecting stroked lines and shapes in a canvas view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class PKLassoToolReference
```

## Overview

A PKLassoToolReference object supports the selection of content on a PKCanvasView. When active, the canvas uses incoming touch events to determine what content to add to the selection.

Create a lasso tool programmatically or display a PKToolPicker object from which the user selects the tool. Assign the resulting object to the tool property of your PKCanvasView object. The canvas uses any subsequent touch sequences to select content on the canvas.

## Topics

### Creating a lasso tool

init()

Creates a lasso tool object for selecting content on a canvas view.

## Relationships

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

