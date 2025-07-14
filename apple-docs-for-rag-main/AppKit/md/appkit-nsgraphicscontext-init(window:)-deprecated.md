

- AppKit
- NSGraphicsContext
-  init(window:) Deprecated

Initializer

# init(window:)

Creates a new graphics context for drawing into a window.

macOS 10.0–10.14Deprecated

``` source
init(window: NSWindow)
```

Deprecated

Add instances of NSView to display content in a window

## Parameters 

`window`  

The window object representing the window to use for drawing.

## Return Value

The created NSGraphicsContext object, or `nil` if the object could not be created.

## See Also

### Creating a Graphics Context

init?(attributes: [NSGraphicsContext.AttributeKey : Any])

Creates a graphics context using the specified attributes.

init?(bitmapImageRep: NSBitmapImageRep)

Creates a new graphics context using the specified bitmap image representation object as the context destination.

init(cgContext: CGContext, flipped: Bool)

Creates a new graphics context from the specified Core Graphics context and the initial flipped state.

init(graphicsPort: UnsafeMutableRawPointer, flipped: Bool)

Creates a new graphics context from the specified graphics port.

Deprecated

