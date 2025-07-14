

- PDFKit
- PDFAnnotationChoiceWidget
-  setFieldName(\_:) Deprecated

Instance Method

# setFieldName(\_:)

Sets the internal field name associated with the widget annotation’s value.

macOS 10.4–10.12Deprecated

``` source
func setFieldName(_ name: String!)
```

## Parameters 

`name`  

The name to be used as the internal field name associated with the widget annotation.

## Discussion

If the widget annotation is backed by PDF form data, it can associate an optional field name with a value or other data.

## See Also

### Managing the Associated Field Name

func fieldName() -> String!

Returns the internal field name associated with the widget annotation.

Deprecated

