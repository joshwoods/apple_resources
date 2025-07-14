

- AppKit
- NSGraphicsContext
-  init(attributes:) 

Initializer

# init(attributes:)

Creates a graphics context using the specified attributes.

macOS

``` source
init?(attributes: [NSGraphicsContext.AttributeKey : Any] = [:])
```

## Parameters 

`attributes`  

A dictionary of values associated with the keys described in NSGraphicsContext.AttributeKey. The attributes specify such things as representation format and destination.

## Return Value

A new NSGraphicsContext object, or `nil` if the object could not be created.

## Discussion

Use this method to create a graphics context for a window or bitmap destination. If you want to create a graphics context for a PDF or PostScript destination, do not use this method; instead, use the NSPrintOperation class to set up the printing environment needed to generate that type of information.

## See Also

### Related Documentation

Cocoa Drawing Guide

### Creating a Graphics Context

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

