

- PDFKit
- PDFAnnotation
-  name(for:) 

Type Method

# name(for:)

Returns the name of the line style, which matches the definition in the Adobe PDF Specification.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
class func name(for style: PDFLineStyle) -> String
```

## Parameters 

`style`  

A line style to get a name for.

## See Also

### Configuring Line Annotations

var startPoint: CGPoint

The point where a line begins, in annotation-space coordinates.

var endPoint: CGPoint

The point where a line ends, in annotation-space coordinates.

var startLineStyle: PDFLineStyle

The style of the line annotation’s starting point, such as square or filled arrowhead.

var endLineStyle: PDFLineStyle

The style of the line annotation’s ending point, such as square or filled arrowhead.

class func lineStyle(fromName: String) -> PDFLineStyle

Returns a line style that corresponds to the specified name.

