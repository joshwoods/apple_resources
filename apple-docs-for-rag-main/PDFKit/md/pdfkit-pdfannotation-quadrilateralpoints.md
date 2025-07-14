

- PDFKit
- PDFAnnotation
-  quadrilateralPoints 

Instance Property

# quadrilateralPoints

An array of values that represents the points bounding the marked-up text.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
var quadrilateralPoints: [NSValue]? { get set }
```

## Discussion

The array contains `N * 4` NSValue objects that use pointValue or cgPointValue to define `N` quadrilaterals in page-space coordinates, where `N` is the number of quad points. The order of the points is a Z pattern as follows:

- Upper-left point

- Upper-right point

- Lower-left point

- Lower-right point

The coordinates of each point are relative to the bound’s origin of the annotation.

## See Also

### Configuring Text Markup Annotations

var markupType: PDFMarkupType

The markup type that the annotation displays, either highlight, strikethrough, underline, or redact.

enum PDFMarkupType

The styles available for markup annotations in PDFKit.

