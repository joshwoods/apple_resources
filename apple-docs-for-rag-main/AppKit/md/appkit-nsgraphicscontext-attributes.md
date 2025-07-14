

- AppKit
- NSGraphicsContext
-  attributes 

Instance Property

# attributes

The attributes used to create this instance.

macOS

``` source
var attributes: [NSGraphicsContext.AttributeKey : Any]? { get }
```

## Discussion

Screen-based graphics contexts do not store attributes, even if you create them using init(attributes:).

## See Also

### Getting Information About the Context

struct AttributeKey

Constants that specify the dictionary keys for the attributes of the graphics context.

struct RepresentationFormatName

Constants that specify values for the representation format name key in a graphic context’s attributes dictionary.

var isFlipped: Bool

A Boolean value that indicates the graphics context’s flipped state.

