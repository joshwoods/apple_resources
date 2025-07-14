

- PencilKit
- PKDrawing
-  dataRepresentation() 

Instance Method

# dataRepresentation()

Returns a raw data representation of the rendered content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 1.0+

``` source
func dataRepresentation() -> Data
```

## Return Value

A new NSData object that contains the entire contents of the drawing.

## See Also

### Getting the drawing data

var strokes: [PKStroke]

The array of strokes that make up the drawing.

let PKAppleDrawingTypeIdentifier: CFString

The uniform type identifier for data associated with a drawing object.

