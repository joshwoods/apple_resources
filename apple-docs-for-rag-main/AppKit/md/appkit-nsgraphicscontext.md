

- AppKit
-  NSGraphicsContext 

Class

# NSGraphicsContext

An object that represents a graphics context.

macOS

``` source
class NSGraphicsContext
```

## Overview

You can think of a graphics context as a destination to which drawing and graphics state operations are sent for execution. Each graphics context contains its own graphics environment and state.

The NSGraphicsContext class is an abstract superclass for destination-specific graphics contexts. You obtain instances of concrete subclasses with the class methods current, init(attributes:), init(bitmapImageRep:), init(cgContext:flipped:), and init(window:).

At any time there is the notion of the current context. The current context for the current thread may be set using current.

Graphics contexts are maintained on a stack. You push a graphics context onto the stack by sending it a saveGraphicsState() message, and pop it off the stack by sending it a restoreGraphicsState() message. By sending restoreGraphicsState() to a graphics context object you remove it from the stack, and the next graphics context on the stack becomes the current graphics context.

## Topics

### Creating a Graphics Context

init?(attributes: [NSGraphicsContext.AttributeKey : Any])

Creates a graphics context using the specified attributes.

init?(bitmapImageRep: NSBitmapImageRep)

Creates a new graphics context using the specified bitmap image representation object as the context destination.

init(cgContext: CGContext, flipped: Bool)

Creates a new graphics context from the specified Core Graphics context and the initial flipped state.

init(window: NSWindow)

Creates a new graphics context for drawing into a window.

Deprecated

init(graphicsPort: UnsafeMutableRawPointer, flipped: Bool)

Creates a new graphics context from the specified graphics port.

Deprecated

### Managing the Current Context

class var current: NSGraphicsContext?

Returns the current graphics context of the current thread.

var cgContext: CGContext

The Core Graphics context, which is a low-level, platform-specific graphics context.

var graphicsPort: UnsafeMutableRawPointer

The low-level, platform-specific graphics context represented by the graphic port.

Deprecated

### Managing the Graphics State

class func restoreGraphicsState()

Pops a graphics context from the per-thread stack, makes it current, and sends the context a restore graphics state message.

func restoreGraphicsState()

Removes the context’s graphics state from the top of the graphics state stack and makes the next graphics state the current graphics state.

class func saveGraphicsState()

Saves the graphics state of the current graphics context.

func saveGraphicsState()

Saves the current graphics state and creates a new graphics state on the top of the stack.

class func setGraphicsState(Int)

Makes the graphics context of the specified graphics state current, and resets graphics state.

Deprecated

### Testing the Drawing Destination

class func currentContextDrawingToScreen() -> Bool

Returns a Boolean value that indicates whether the current context is drawing to the screen.

var isDrawingToScreen: Bool

A Boolean value that indicates whether the drawing destination is the screen.

### Getting Information About the Context

var attributes: [NSGraphicsContext.AttributeKey : Any]?

The attributes used to create this instance.

struct AttributeKey

Constants that specify the dictionary keys for the attributes of the graphics context.

struct RepresentationFormatName

Constants that specify values for the representation format name key in a graphic context’s attributes dictionary.

var isFlipped: Bool

A Boolean value that indicates the graphics context’s flipped state.

### Flushing Graphics to the Context

func flushGraphics()

Forces any buffered operations or data to be sent to the graphics context’s destination.

### Configuring Rendering Options

var compositingOperation: NSCompositingOperation

The graphics context’s global compositing operation setting.

enum NSCompositingOperation

Constants that describe compositing operators in terms of source and destination images, each having an opaque and transparent region.

var imageInterpolation: NSImageInterpolation

A constant that specifies the graphics context’s interpolation, or image smoothing, behavior.

enum NSImageInterpolation

Constants that specify the interpolation, or image smoothing, behavior used by the image interpolation property.

var shouldAntialias: Bool

A Boolean value that indicates whether the graphics context uses antialiasing.

var patternPhase: NSPoint

The amount to offset the pattern color when filling the graphics context.

### Getting the Context for Rendering Core Image Objects

var ciContext: CIContext?

A context for Core Image objects that you can use to render into the graphics context.

### Managing Color Rendering

var colorRenderingIntent: NSColorRenderingIntent

The color rendering intent in the graphics context’s graphics state.

enum NSColorRenderingIntent

Constants that specify how Cocoa should handle colors that are not located within the destination color space of a graphics context.

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

