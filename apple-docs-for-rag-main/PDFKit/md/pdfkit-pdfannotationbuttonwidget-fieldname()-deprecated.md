

- PDFKit
- PDFAnnotationButtonWidget
-  fieldName() Deprecated

Instance Method

# fieldName()

Returns the internal name of a field (used for reset-form actions).

macOS 10.4–10.12Deprecated

``` source
func fieldName() -> String!
```

## Return Value

The internal name of a field.

## Discussion

The internal name of a field is an optional value.

## See Also

### Related Documentation

class PDFAnnotationButtonWidget

A `PDFAnnotationButtonWidget` object provides user interactivity on a page of a PDF document. There are three types of buttons available: push button, radio button, and checkbox.

Deprecated

### Managing Control State Values and Form Fields

func onStateValue() -> String!

Returns the string associated with the on state of a radio button or checkbox control.

Deprecated

func setOnStateValue(String!)

Sets the string that is associated with the on state of a radio button or checkbox control.

Deprecated

func setFieldName(String!)

Sets the internal name of a field (used for reset-form actions).

Deprecated

