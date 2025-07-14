

- AppKit
- NSGraphicsContext
-  init(bitmapImageRep:) 

Initializer

# init(bitmapImageRep:)

Creates a new graphics context using the specified bitmap image representation object as the context destination.

macOS

``` source
init?(bitmapImageRep bitmapRep: NSBitmapImageRep)
```

## Parameters 

`bitmapRep`  

The NSBitmapImageRep object to use as the destination.

## Return Value

The created NSGraphicsContext object, or `nil` if the object could not be created.

## Discussion

This method accepts only single plane NSBitmapImageRep instances. It is the equivalent of using init(attributes:) and passing `bitmapRep` as the value for the dictionary’s destination key.

## See Also

### Creating a Graphics Context

init?(attributes: [NSGraphicsContext.AttributeKey : Any])

Creates a graphics context using the specified attributes.

init(cgContext: CGContext, flipped: Bool)

Creates a new graphics context from the specified Core Graphics context and the initial flipped state.

init(window: NSWindow)

Creates a new graphics context for drawing into a window.

Deprecated

init(graphicsPort: UnsafeMutableRawPointer, flipped: Bool)

Creates a new graphics context from the specified graphics port.

Deprecated

