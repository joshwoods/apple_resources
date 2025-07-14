

- AppKit
- Drawing
-  Convenience Functions 

API Collection

# Convenience Functions

Draw rectangles and other primitive shapes using these convenience functions.

## Topics

### Drawing Rectangles

func NSEraseRect(NSRect)

Erases the specified rect by filling it with white.

func NSDrawTiledRects(NSRect, NSRect, UnsafePointer&lt;NSRectEdge>, UnsafePointer&lt;CGFloat>, Int) -> NSRect

Draws rectangles with borders.

func NSDrawGroove(NSRect, NSRect)

Draws a gray-filled rectangle with a groove border.

### Drawing Bezels

func NSDrawDarkBezel(NSRect, NSRect)

Draws a dark gray-filled rectangle with a bezel border.

func NSDrawGrayBezel(NSRect, NSRect)

Draws a gray-filled rectangle with a bezel border.

func NSDrawLightBezel(NSRect, NSRect)

Draws a white-filled rectangle with a bezel border.

func NSDrawWhiteBezel(NSRect, NSRect)

Draws a white-filled rectangle with a bezel border.

### Drawing Backgrounds

func NSDrawButton(NSRect, NSRect)

Draws a gray-filled rectangle representing a user-interface button.

func NSDrawWindowBackground(NSRect)

Draws the window’s default background pattern into the specified rectangle of the currently focused view.

### Drawing Multipart Images

func NSDrawNinePartImage(NSRect, NSImage?, NSImage?, NSImage?, NSImage?, NSImage?, NSImage?, NSImage?, NSImage?, NSImage?, NSCompositingOperation, CGFloat, Bool)

Draws a nine-part tiled image.

func NSDrawThreePartImage(NSRect, NSImage?, NSImage?, NSImage?, Bool, NSCompositingOperation, CGFloat, Bool)

Draws a three-part tiled image.

### Drawing Focus Rings

func set()

Specifies how the system draws the focus ring.

enum NSFocusRingPlacement

Constants that indicate how the system draws the focus ring.

enum NSFocusRingType

Constants that describe the style of the focus ring.

## See Also

### Shapes and Paths

class NSBezierPath

An object that can create paths using PostScript-style commands.

