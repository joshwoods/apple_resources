

- PDFKit
- PDFAnnotationChoiceWidget
-  setStringValue(\_:) Deprecated

Instance Method

# setStringValue(\_:)

Sets the selection in the widget annotation.

macOS 10.4–10.12Deprecated

``` source
func setStringValue(_ value: String!)
```

## Parameters 

`value`  

The string that represents the selection in the widget annotation.

## Discussion

If the widget annotation object is backed by PDF form data, this method updates the value associated with the appropriate field in the form object.

## See Also

### Getting and Setting the String Value

func stringValue() -> String!

Returns the selection in the widget annotation.

Deprecated

