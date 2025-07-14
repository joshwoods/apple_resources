

- SwiftUI
-  PointerStyle 

Structure

# PointerStyle

A style describing the appearance of the pointer (also called a cursor) when it’s hovered over a view.

macOS 15.0+visionOS 2.0+

``` source
struct PointerStyle
```

## Overview

Use the pointerStyle(_:) view modifier to set a view’s pointer style.

For guidance on choosing an appropriate pointer style, refer to Pointing devices in the Human Interface Guidelines.

## Topics

### Type Properties

static let columnResize: PointerStyle

The pointer style for resizing a column, or vertical division, in either direction.

static let `default`: PointerStyle

The pointer style that uses the default platform appearance.

static let grabActive: PointerStyle

The pointer style appropriate for actively dragging to reposition content within specific bounds, such as panning a large image.

static let grabIdle: PointerStyle

The pointer style appropriate to indicate that dragging to reposition content within specific bounds, such as panning a large image, is possible.

static let horizontalText: PointerStyle

The pointer style appropriate for selecting or inserting text in a horizontal layout.

static let link: PointerStyle

The pointer style appropriate for content opens a URL link to a webpage, document, or other item when clicked.

static let rectSelection: PointerStyle

The pointer style appropriate for precise rectangular selection, such as selecting a portion of an image or multiple lines of text.

static let rowResize: PointerStyle

The pointer style for resizing a row, or horizontal division, in either direction.

static let verticalText: PointerStyle

The pointer style appropriate for selecting or inserting text in a vertical layout.

static let zoomIn: PointerStyle

The pointer style appropriate to indicate that the content can be zoomed in.

static let zoomOut: PointerStyle

The pointer style appropriate to indicate that the content can be zoomed out.

### Type Methods

static func columnResize(directions: HorizontalDirection.Set) -> PointerStyle

The pointer style for resizing a column, or vertical division.

static func frameResize(position: FrameResizePosition, directions: FrameResizeDirection.Set) -> PointerStyle

The pointer style for resizing a rectangular frame from a specific edge or corner.

static image(_:hotSpot:)

Initializes a pointer style with a given image and hot spot.

static func rowResize(directions: VerticalDirection.Set) -> PointerStyle

The pointer style for resizing a row, or horizontal division.

static func shape(some Shape, eoFill: Bool, size: CGSize) -> PointerStyle

Initializes a pointer style with a given shape.

## Relationships

### Conforms To

- Sendable

## See Also

### Modifying pointer appearance

func pointerStyle(PointerStyle?) -> some View

Sets the pointer style to display when the pointer is over the view.

func pointerVisibility(Visibility) -> some View

Sets the visibility of the pointer when it’s over the view.

enum HorizontalDirection

A direction on the horizontal axis.

enum VerticalDirection

A direction on the horizontal axis.

enum FrameResizePosition

The position along the perimeter of a rectangular frame (its edges and corners) from which it’s resized.

enum FrameResizeDirection

The direction in which a rectangular frame can be resized.

