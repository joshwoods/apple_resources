

- PencilKit
-  PKCanvasView 

Class

# PKCanvasView

A view that captures Apple Pencil input and displays the rendered results in an iOS app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class PKCanvasView
```

## Mentioned in 

Supporting backward compatibility for ink types

## Overview

A PKCanvasView object captures content drawn using Apple Pencil or the user’s finger and displays it in your app. The canvas view handles all of the touch events and data coming from Apple Pencil, and renders that information using the tool you specify. The canvas stores the captured input in a PKDrawingReference object.

PKCanvasView is a scroll view, so you can make the drawable area bigger than the canvas view’s frame rectangle. To do that, set the inherited contentSize property to the size you want. The canvas view automatically scales its underlying content to match the size you specify. Users scroll around the canvas using a two-finger pan gesture. (If the allowsFingerDrawing property is `false`, users scroll with only one finger.)

A canvas view conforms to the PKToolPickerObserver protocol, so you can add it as an observer of the window’s tool picker. The tool picker displays a floating palette of tools that the user can choose from. As the user interacts with items in the palette, such as changing ink colors, or line widths, the canvas automatically updates its drawing environment accordingly.

## Topics

### Responding to drawing-related changes

var delegate: (any PKCanvasViewDelegate)?

The object you use to respond to changes in the drawn content or with the selected tool.

protocol PKCanvasViewDelegate

Methods for monitoring drawing related changes in a canvas view.

### Configuring the drawing environment

var tool: any PKTool

The currently selected tool used for drawing.

var isRulerActive: Bool

A Boolean value that indicates whether a ruler view is visible on the canvas.

var allowsFingerDrawing: Bool

A Boolean value that indicates whether the canvas accepts input from the user’s finger in addition to Apple Pencil.

Deprecated

var drawingPolicy: PKCanvasViewDrawingPolicy

The policy that controls the types of touches allowed when drawing on the canvas.

enum PKCanvasViewDrawingPolicy

Constants that you use to specify the type of drawing gestures your app permits while the user draws on the canvas.

### Getting the drawing gesture recognizer

var drawingGestureRecognizer: UIGestureRecognizer

The gesture recognizer that the canvas uses to track touch events.

### Getting the captured data

var drawing: PKDrawing

The data object that the canvas uses to store drawn content.

### Supporting PencilKit versions

var maximumSupportedContentVersion: PKContentVersion

The maximum version of PencilKit to support.

### Instance Properties

var isDrawingEnabled: Bool

## Relationships

### Inherits From

- UIScrollView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- PKToolPickerObserver
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIFocusItemScrollableContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Canvas

Drawing with PencilKit

Add expressive, low-latency drawing to your app using PencilKit.

Customizing Scribble with Interactions

Enable writing on a non-text-input view by adding interactions.

Inspecting, Modifying, and Constructing PencilKit Drawings

Score users’ ability to match PencilKit drawings generated from text, by accessing the strokes and points inside PencilKit drawings.

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

