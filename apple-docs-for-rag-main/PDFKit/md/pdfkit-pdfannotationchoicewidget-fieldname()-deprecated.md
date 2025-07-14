

- PDFKit
- PDFAnnotationChoiceWidget
-  fieldName() Deprecated

Instance Method

# fieldName()

Returns the internal field name associated with the widget annotation.

macOS 10.4–10.12Deprecated

``` source
func fieldName() -> String!
```

## Return Value

The internal field name associated with the widget annotation.

## Discussion

If the widget annotation is backed by PDF form data, it can associate an optional field name with a value or other data.

## See Also

### Managing the Associated Field Name

func setFieldName(String!)

Sets the internal field name associated with the widget annotation’s value.

Deprecated

