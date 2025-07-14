

- UIKit
-  NSTextViewportLayoutController 

Class

# NSTextViewportLayoutController

Manages the layout process inside the viewport interacting with its delegate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
class NSTextViewportLayoutController
```

## Overview

A viewport is a rectangular area within a flipped coordinate system expanding along the y-axis. With text contents, lines advance expanding the view in the current writing direction. The viewport defines the active area where the framework lays out text fragments. In most cases, the area corresponds to the user visible area with an additional over-scroll region.

## Topics

### Creating a viewport layout controller

init(textLayoutManager: NSTextLayoutManager)

Creates a new instance with the text layout manager you provide.

### Accessing the layout manager

var textLayoutManager: NSTextLayoutManager?

Returns the text layout manager for this viewport layout controller.

### Responding to changes in viewport layout

var delegate: (any NSTextViewportLayoutControllerDelegate)?

The delegate for the text layout manager object.

protocol NSTextViewportLayoutControllerDelegate

Optional methods that delegates implement to respond to viewport layout changes.

### Accessing the viewport characteristics

var viewportBounds: CGRect

Returns the visible bounds of the view, plus the overdraw area.

var viewportRange: NSTextRange?

Returns the text range of the current viewport layout.

func adjustViewport(byVerticalOffset: CGFloat)

Adjusts the viewport rect by the specified offset if needed.

func layoutViewport()

Performs layout in the viewport.

func relocateViewport(to: any NSTextLocation) -> CGFloat

Relocates the viewport to the location you specify.

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

### Layout

Using TextKit 2 to interact with text

Interact with text by managing text selection and inserting custom text elements.

Display text with a custom layout

Lay out text in a custom-shaped container and apply glyph substitutions.

class NSTextLayoutManager

The primary class that you use to manage text layout and presentation for custom text displays.

class NSTextContainer

A region where text layout occurs.

class NSTextLayoutFragment

A class that represents the layout fragment typically corresponding to a rendering surface, such as a layer or view subclass.

class NSTextLineFragment

A class that represents a line fragment as a single textual layout and rendering unit inside a text layout fragment.

protocol NSTextLayoutOrientationProvider

A set of methods that define the orientation of text for an object.

