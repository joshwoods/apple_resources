

- PDFKit
- PDFAnnotation
-  value(forAnnotationKey:) 

Instance Method

# value(forAnnotationKey:)

Returns a deep copy of the key-value pairs of properties for the specified key.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+

``` source
func value(forAnnotationKey key: PDFAnnotationKey) -> Any?
```

## Parameters 

`key`  

A PDFAnnotationKey or appropriate string from the Adobe PDF Specification.

## See Also

### Modifying Annotation Attributes

var annotationKeyValues: [AnyHashable : Any]

A dictionary that contains a deep copy of the widget’s properties.

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

