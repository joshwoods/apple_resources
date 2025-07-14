

- PencilKit
- PKDrawingReference
-  dataRepresentation() 

Instance Method

# dataRepresentation()

Returns a representation of the rendered content as data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func dataRepresentation() -> Data
```

## Return Value

A new NSData object that contains the entire contents of the drawing.

## See Also

### Getting the drawing data

var strokes: [PKStroke]

An array of strokes used to represent the drawing.

let PKAppleDrawingTypeIdentifier: CFString

The uniform type identifier for data associated with a drawing object.

