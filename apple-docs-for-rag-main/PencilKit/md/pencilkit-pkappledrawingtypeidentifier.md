

- PencilKit
-  PKAppleDrawingTypeIdentifier 

Global Variable

# PKAppleDrawingTypeIdentifier

The uniform type identifier for data associated with a drawing object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
let PKAppleDrawingTypeIdentifier: CFString
```

## Discussion

Use this type when reading or writing drawing data. For example, use this type to determine if you can read data from the pasteboard.

## See Also

### Getting the drawing data

var strokes: [PKStroke]

The array of strokes that make up the drawing.

func dataRepresentation() -> Data

Returns a raw data representation of the rendered content.

