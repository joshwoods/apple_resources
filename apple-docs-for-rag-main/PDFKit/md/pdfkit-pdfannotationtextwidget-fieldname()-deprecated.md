

- PDFKit
- PDFAnnotationTextWidget
-  fieldName() Deprecated

Instance Method

# fieldName()

Returns the internal name for the annotation text field.

macOS 10.4–10.12Deprecated

``` source
func fieldName() -> String!
```

## Return Value

The internal name for the annotation text field.

## Discussion

Field names are optional, internal names that identify text fields in a PDF form. You use field names with the PDFActionResetForm action.

Note that multiple `PDFAnnotationTextWidget` objects with the same field name always have the same text associated with that field name. When text is entered into one of the objects, the text associated with that field name is changed in all objects. If you need to ensure unique text for a `PDFAnnotationTextWidget` object, you must give it a unique field name (you can use setFieldName(_:) to do this).

## See Also

### Related Documentation

class PDFAnnotationTextWidget

A `PDFAnnotationTextWidget` object allows you to manage the appearance and content of text fields.

Deprecated

### Working with Field Names

func setFieldName(String!)

Sets the internal field name for the annotation text field.

Deprecated

