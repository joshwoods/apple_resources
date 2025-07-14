

- PDFKit
- PDFAnnotation
-  setValue(\_:forAnnotationKey:) 

Instance Method

# setValue(\_:forAnnotationKey:)

Sets a value in the annotation’s dictionary.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+

``` source
func setValue(
    _ value: Any,
    forAnnotationKey key: PDFAnnotationKey
) -> Bool
```

## Parameters 

`value`  

The value to set in the attribute’s dictionary.

`key`  

A PDFAnnotationKey or appropriate string from the Adobe PDF Specification.

## Return Value

true if the value sets successfully; otherwise, false.

## Discussion

Some keys expect a complex type. For example, the color key expects an array of zero, one, two, three, or four elements, where each element is a floating-point number from `0.0` to `1.0`. As a convenience, this key accepts an NSColor or UIColor value. For details about other conveniences, see the individual PDFAnnotationKey properties or the `PDFAnnotationUtilities.h` header file.

Tip

Set the `PDFKIT_LOG_ANNOTATIONS` environment variable to log key-value assignment failure details.

## See Also

### Modifying Annotation Attributes

var annotationKeyValues: [AnyHashable : Any]

A dictionary that contains a deep copy of the widget’s properties.

func value(forAnnotationKey: PDFAnnotationKey) -> Any?

Returns a deep copy of the key-value pairs of properties for the specified key.

func setBoolean(Bool, forAnnotationKey: PDFAnnotationKey) -> Bool

Sets a Boolean value in the annotation’s dictionary.

func setRect(CGRect, forAnnotationKey: PDFAnnotationKey) -> Bool

Sets a rectangle value in the annotation’s dictionary.

func removeValue(forAnnotationKey: PDFAnnotationKey)

Removes a value from the annotation’s dictionary.

struct PDFAnnotationKey

Keys for setting properties of annotations.

