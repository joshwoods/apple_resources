

- AppKit
-  NSRulerMarker 

Class

# NSRulerMarker

A symbol on a ruler view, indicating a location for the graphics element it represents in the client of the ruler view.

macOS

``` source
class NSRulerMarker
```

## Overview

An example of a marker is the representation of a margin or tab setting, or the edges of a graphic on the page.

## Topics

### Creating instances

init(rulerView: NSRulerView, markerLocation: CGFloat, image: NSImage, imageOrigin: NSPoint)

Initializes a newly allocated ruler marker, associating it with (but not adding it to) a specified ruler view and assigning the attributes provided.

### Getting the ruler view

var ruler: NSRulerView?

The receiver’s ruler view.

### Setting the image

var image: NSImage

The receiver’s image.

var imageOrigin: NSPoint

The point in the receiver’s image that is positioned at the receiver’s location on the ruler view.

var imageRectInRuler: NSRect

The rectangle occupied by the receiver’s image.

var thicknessRequiredInRuler: CGFloat

The amount of the receiver’s image that’s displayed above or to the left of the ruler view’s baseline.

### Setting movability

var isMovable: Bool

A Boolean that indicates whether the user can move the receiver in its ruler view.

var isRemovable: Bool

A Boolean that indicates whether the user can remove the receiver from its ruler view.

### Setting the location

var markerLocation: CGFloat

The location of the receiver in the coordinate system of the ruler view’s client view.

### Setting the represented object

var representedObject: (any NSCopying)?

The object the receiver represents.

### Drawing and event handling

func draw(NSRect)

Draws the receiver’s image that appears in the supplied rectangle.

var isDragging: Bool

A Boolean that indicates whether the receiver is being dragged.

func trackMouse(with: NSEvent, adding: Bool) -> Bool

Handles user manipulation of the receiver in its ruler view.

### Initializers

init(coder: NSCoder)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Rulers

class NSRulerView

A ruler and the markers above or to the side of a scroll view’s document view.

