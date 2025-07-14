

- PDFKit
- PDFAnnotation
-  init(bounds:forType:withProperties:) 

Initializer

# init(bounds:forType:withProperties:)

Creates a PDF annotation with the specified bounds, type, and optional properties.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
init(
    bounds: CGRect,
    forType annotationType: PDFAnnotationSubtype,
    withProperties properties: [AnyHashable : Any]?
)
```

**macOS**

``` source
init(
    bounds: NSRect,
    forType annotationType: PDFAnnotationSubtype,
    withProperties properties: [AnyHashable : Any]?
)
```

## Parameters 

`bounds`  

The bounding box of the annotation, in page-space coordinates.

`annotationType`  

The subtype of the annotation, such as text, link, or line.

`properties`  

A dictionary that contains properties of the annotation.

## See Also

### Creating an Annotation

struct PDFAnnotationSubtype

The type of annotation, such as circle, text, or ink.

