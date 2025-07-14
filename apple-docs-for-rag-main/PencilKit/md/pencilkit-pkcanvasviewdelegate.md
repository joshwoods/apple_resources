

- PencilKit
-  PKCanvasViewDelegate 

Protocol

# PKCanvasViewDelegate

Methods for monitoring drawing related changes in a canvas view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol PKCanvasViewDelegate : UIScrollViewDelegate
```

## Overview

Implement the methods of the PKCanvasViewDelegate protocol to monitor drawing events in a PKCanvasView object. Specifically, determine the start- and end-of-event sequences using the currently selected tool, and determine when those events affect the drawn content.

## Topics

### Responding to drawing-related changes

func canvasViewDrawingDidChange(PKCanvasView)

Tells the delegate that the contents of the current drawing changed.

func canvasViewDidFinishRendering(PKCanvasView)

Tells the delegate that the previously drawn content is ready to display.

### Responding to new event sequences

func canvasViewDidBeginUsingTool(PKCanvasView)

Tells the delegate that the user started a new drawing sequence with the currently selected tool.

func canvasViewDidEndUsingTool(PKCanvasView)

Tells the delegate that the user ended a drawing sequence with the tool they were using.

## Relationships

### Inherits From

- NSObjectProtocol
- UIScrollViewDelegate

## See Also

### Responding to drawing-related changes

var delegate: (any PKCanvasViewDelegate)?

The object you use to respond to changes in the drawn content or with the selected tool.

