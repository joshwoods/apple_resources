

- PencilKit
-  PKToolPicker 

Class

# PKToolPicker

A tool palette that displays a selection of drawing tools and colors for tools that a person can choose from.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class PKToolPicker
```

## Mentioned in 

Supporting backward compatibility for ink types

## Overview

A PKToolPicker manages a draggable palette that displays drawing tools, colors, and additional options. You add a tool picker to your interface and configure it to display its palette at appropriate times. While the palette is onscreen, a person may reposition it anywhere within the current window. When a person interacts with the palette, the tool picker notifies registered observers of the changes so that they can respond.

Important

The tool picker doesn’t display in Mac apps built with Mac Catalyst.

When configuring your interface, call the setVisible(_:forFirstResponder:) method to associate the tool picker with one or more views in your interface. Each window manages its own tool picker, and the window’s first responder determines the visibility of that tool picker. When one of the registered objects becomes first responder, the tool picker automatically adds its palette view to the current window. When there isn’t a registered object as first responder, the tool picker hides its palette view.

PKCanvasView implements the observer protocol for detecting tool picker changes. Adding your canvas view as an observer to a tool picker automatically updates the current drawing tools. For more information about implementing custom observer objects, see PKToolPickerObserver.

## Topics

### Creating a tool picker

init()

Creates a new tool picker with a default set of tools.

init(toolItems: [PKToolPickerItem])

Creates a new tool picker with the tools you specify.

class PKToolPickerInkingItem

An item that represents an inking tool in the tool picker.

class PKToolPickerEraserItem

An item that represents an eraser tool in the tool picker.

class PKToolPickerLassoItem

An item that represents a lasso tool in the tool picker.

class PKToolPickerRulerItem

An item that represents a ruler tool in the tool picker.

class PKToolPickerScribbleItem

An item that represents a Scribble tool in the tool picker.

class PKToolPickerCustomItem

An item that represents a custom tool in the tool picker.

class PKToolPickerItem

The base class for an item in the tool picker.

### Accessing the picker’s tools

var toolItems: [PKToolPickerItem]

All tool items in the tool picker.

### Detecting changes to the picker

func addObserver(any PKToolPickerObserver)

Adds the specified object to the list of objects to notify when the picker configuration changes.

func removeObserver(any PKToolPickerObserver)

Removes the specified object from the list of objects to notify when the picker configuration changes.

protocol PKToolPickerObserver

An interface you use to detect when the user changes the selected tools and drawing characteristics of a tool picker object.

### Coordinating the visibility of the picker

func setVisible(Bool, forFirstResponder: UIResponder)

Sets the visibility for the tool picker, based on when the specified responder object becomes active.

var isVisible: Bool

A Boolean value that indicates whether the tool picker is currently visible.

func frameObscured(in: UIView) -> CGRect

Returns the portion of the specified view that the tool picker obscures.

### Managing selected tools

var selectedToolItem: PKToolPickerItem

The currently selected tool item in the tool picker.

var selectedToolItemIdentifier: String

The identifier of the selected tool item in the tool picker.

### Customizing picker behavior

var isRulerActive: Bool

A Boolean value that indicates whether the ruler is visible on the canvas.

var colorUserInterfaceStyle: UIUserInterfaceStyle

The user interface style for the tool picker.

var overrideUserInterfaceStyle: UIUserInterfaceStyle

The specific user interface style to apply to the tool picker.

var showsDrawingPolicyControls: Bool

A Boolean value that indicates whether the default drawing policy UI is visible.

var stateAutosaveName: String?

The name used to automatically save the tool picker’s state in the defaults system.

### Configuring the accessory item

var accessoryItem: UIBarButtonItem?

An optional button that appears at the trailing edge of the tool picker.

### Supporting PencilKit versions

var maximumSupportedContentVersion: PKContentVersion

The maximum version of PencilKit to support.

### Deprecated

class func shared(for: UIWindow) -> PKToolPicker?

Returns the tool picker object to use for the specified window.

Deprecated

var selectedTool: any PKTool

The currently selected tool in the tool picker.

Deprecated

### Protocols

protocol Delegate

### Instance Properties

var delegate: (any PKToolPicker.Delegate)?

The delegate for the tool picker.

var prefersDismissControlVisible: Bool

If this is true the tool picker may show UI that allows dismissing it. If this is false the tool picker will not show this UI. By default this resigns first responder, but is customizable by `PKToolPickerDelegate`’s `toolPickerWillDismiss...` method.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Tools

Configuring the PencilKit tool picker

Incorporate a custom PencilKit tool picker with a variety of system and custom tools into a drawing app.

struct PKInkingTool

A structure that defines the drawing characteristics (width, color, pen style) to use when drawing lines on a canvas view.

struct PKEraserTool

A tool for erasing previously drawn content in a canvas view.

struct PKLassoTool

A tool for selecting stroked lines and shapes in a canvas view.

protocol PKTool

An interface adopted by drawing and writing tools used by a canvas view.

