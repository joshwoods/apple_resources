

- PDFKit
- PDFAnnotation
-  annotationKeyValues 

Instance Property

# annotationKeyValues

A dictionary that contains a deep copy of the widget’s properties.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var annotationKeyValues: [AnyHashable : Any] { get }
```

## See Also

### Modifying Annotation Attributes

func value(forAnnotationKey: PDFAnnotationKey) -> Any?

Returns a deep copy of the key-value pairs of properties for the specified key.

func setValue(Any, forAnnotationKey: PDFAnnotationKey) -> Bool

Sets a value in the annotation’s dictionary.

func setBoolean(Bool, forAnnotationKey: PDFAnnotationKey) -> Bool

Sets a Boolean value in the annotation’s dictionary.

func setRect(CGRect, forAnnotationKey: PDFAnnotationKey) -> Bool

Sets a rectangle value in the annotation’s dictionary.

func removeValue(forAnnotationKey: PDFAnnotationKey)

Removes a value from the annotation’s dictionary.

struct PDFAnnotationKey

Keys for setting properties of annotations.

