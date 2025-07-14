

- AppKit
- NSGraphicsContext
-  init(cgContext:flipped:) 

Initializer

# init(cgContext:flipped:)

Creates a new graphics context from the specified Core Graphics context and the initial flipped state.

macOS 10.10+

``` source
init(
    cgContext graphicsPort: CGContext,
    flipped initialFlippedState: Bool
)
```

## Parameters 

`graphicsPort`  

The graphics port used to create the graphics-context object, as a CGContext (opaque type) object.

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

init(window: NSWindow)

Creates a new graphics context for drawing into a window.

Deprecated

init(graphicsPort: UnsafeMutableRawPointer, flipped: Bool)

Creates a new graphics context from the specified graphics port.

Deprecated

