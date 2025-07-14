

- AppKit
- NSGraphicsContext
-  isFlipped 

Instance Property

# isFlipped

A Boolean value that indicates the graphics context’s flipped state.

macOS

``` source
var isFlipped: Bool { get }
```

## Discussion

The state is determined by sending `flipped` to the receiver’s view that has focus. If no view has focus, returns false unless the receiver is instantiated using init(cgContext:flipped:) specifying true as the `flipped` parameter.

## See Also

### Related Documentation

init(cgContext: CGContext, flipped: Bool)

Creates a new graphics context from the specified Core Graphics context and the initial flipped state.

### Getting Information About the Context

var attributes: [NSGraphicsContext.AttributeKey : Any]?

The attributes used to create this instance.

struct AttributeKey

Constants that specify the dictionary keys for the attributes of the graphics context.

struct RepresentationFormatName

Constants that specify values for the representation format name key in a graphic context’s attributes dictionary.

