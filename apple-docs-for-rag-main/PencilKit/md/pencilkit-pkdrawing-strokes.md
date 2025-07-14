

- PencilKit
- PKDrawing
-  strokes 

Instance Property

# strokes

The array of strokes that make up the drawing.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var strokes: [PKStroke] { get set }
```

## See Also

### Getting the drawing data

func dataRepresentation() -> Data

Returns a raw data representation of the rendered content.

let PKAppleDrawingTypeIdentifier: CFString

The uniform type identifier for data associated with a drawing object.

