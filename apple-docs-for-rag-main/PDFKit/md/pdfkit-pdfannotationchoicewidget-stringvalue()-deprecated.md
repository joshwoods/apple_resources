

- PDFKit
- PDFAnnotationChoiceWidget
-  stringValue() Deprecated

Instance Method

# stringValue()

Returns the selection in the widget annotation.

macOS 10.4–10.12Deprecated

``` source
func stringValue() -> String!
```

## Return Value

The string that represents the selection in the widget annotation.

## Discussion

If the widget annotation object is backed by PDF form data, this method returns the value associated with the appropriate field in the form object, if possible.

## See Also

### Getting and Setting the String Value

func setStringValue(String!)

Sets the selection in the widget annotation.

Deprecated

