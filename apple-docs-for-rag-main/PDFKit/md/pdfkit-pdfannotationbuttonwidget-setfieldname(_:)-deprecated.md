

- PDFKit
- PDFAnnotationButtonWidget
-  setFieldName(\_:) Deprecated

Instance Method

# setFieldName(\_:)

Sets the internal name of a field (used for reset-form actions).

macOS 10.4–10.12Deprecated

``` source
func setFieldName(_ name: String!)
```

## Parameters 

`name`  

The internal name of a field. This is an optional value.

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

func fieldName() -> String!

Returns the internal name of a field (used for reset-form actions).

Deprecated

