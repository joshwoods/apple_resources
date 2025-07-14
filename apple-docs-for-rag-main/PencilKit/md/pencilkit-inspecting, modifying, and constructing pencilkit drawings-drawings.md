

- PencilKit
-  Inspecting, Modifying, and Constructing PencilKit Drawings 

Sample Code

# Inspecting, Modifying, and Constructing PencilKit Drawings

Score users’ ability to match PencilKit drawings generated from text, by accessing the strokes and points inside PencilKit drawings.

Download

iOS 14.0+iPadOS 14.0+Xcode 11.5+

## Overview

Note

This sample code project is associated with WWDC20 session 10148: Inspect, Modify, and Construct PencilKit Drawings.

This sample code project must be run on a physical device with Apple Pencil.

## See Also

### Canvas

Drawing with PencilKit

Add expressive, low-latency drawing to your app using PencilKit.

Customizing Scribble with Interactions

Enable writing on a non-text-input view by adding interactions.

class PKCanvasView

A view that captures Apple Pencil input and displays the rendered results in an iOS app.

struct PKDrawing

A structure representing the drawing information captured by a canvas view.

struct PKStroke

A structure that represents the paths, boundaries, and other properties of a stroke drawn on a canvas.

struct PKStrokePath

A structure that captures the components of a stroke and provides methods to find and interpolate points along the stroke’s path.

struct PKStrokePoint

A structure that represents the properties of a specific point along a stroke’s path.

struct PKInk

A structure that represents an ink that specifies its type, color, and width.

