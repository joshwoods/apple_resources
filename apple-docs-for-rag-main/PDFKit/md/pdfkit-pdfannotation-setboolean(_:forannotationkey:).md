

- PDFKit
- PDFAnnotation
-  setBoolean(\_:forAnnotationKey:) 

Instance Method

# setBoolean(\_:forAnnotationKey:)

Sets a Boolean value in the annotation’s dictionary.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+

``` source
func setBoolean(
    _ value: Bool,
    forAnnotationKey key: PDFAnnotationKey
) -> Bool
```

## Parameters 

`value`  

The Boolean value to set in the annotation’s dictionary.

`key`  

A PDFAnnotationKey or appropriate string from the Adobe PDF Specification.

## Return Value

true if the value sets successfully; otherwise, false.

## See Also

### Modifying Annotation Attributes

var annotationKeyValues: [AnyHashable : Any]

A dictionary that contains a deep copy of the widget’s properties.

func value(forAnnotationKey: PDFAnnotationKey) -> Any?

Returns a deep copy of the key-value pairs of properties for the specified key.

func setValue(Any, forAnnotationKey: PDFAnnotationKey) -> Bool

Sets a value in the annotation’s dictionary.

func setRect(CGRect, forAnnotationKey: PDFAnnotationKey) -> Bool

Sets a rectangle value in the annotation’s dictionary.

func removeValue(forAnnotationKey: PDFAnnotationKey)

Removes a value from the annotation’s dictionary.

struct PDFAnnotationKey

Keys for setting properties of annotations.

