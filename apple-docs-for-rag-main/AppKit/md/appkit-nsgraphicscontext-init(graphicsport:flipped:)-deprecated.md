

- AppKit
- NSGraphicsContext
-  init(graphicsPort:flipped:) Deprecated

Initializer

# init(graphicsPort:flipped:)

Creates a new graphics context from the specified graphics port.

macOS 10.0–10.14Deprecated

``` source
init(
    graphicsPort: UnsafeMutableRawPointer,
    flipped initialFlippedState: Bool
)
```

Deprecated

Use init(cgContext:flipped:) instead.

## Parameters 

`graphicsPort`  

The graphics port used to create the graphics-context object. Typically `graphicsPort` is a CGContext (opaque type) object.

`initialFlippedState`  

Specifies the receiver’s initial flipped state. This is the value returned by isFlipped when no view has focus.

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

init(window: NSWindow)

Creates a new graphics context for drawing into a window.

Deprecated

