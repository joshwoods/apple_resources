

- PDFKit
- PDFAnnotation
-  endPoint 

Instance Property

# endPoint

The point where a line ends, in annotation-space coordinates.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
var endPoint: CGPoint { get set }
```

**macOS**

``` source
var endPoint: NSPoint { get set }
```

## See Also

### Configuring Line Annotations

var startPoint: CGPoint

The point where a line begins, in annotation-space coordinates.

var startLineStyle: PDFLineStyle

The style of the line annotation’s starting point, such as square or filled arrowhead.

var endLineStyle: PDFLineStyle

The style of the line annotation’s ending point, such as square or filled arrowhead.

class func lineStyle(fromName: String) -> PDFLineStyle

Returns a line style that corresponds to the specified name.

class func name(for: PDFLineStyle) -> String

Returns the name of the line style, which matches the definition in the Adobe PDF Specification.

