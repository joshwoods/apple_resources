

- PDFKit
- PDFAnnotationTextWidget
-  setMaximumLength(\_:) Deprecated

Instance Method

# setMaximumLength(\_:)

Sets the maximum number of characters allowed in the annotation string.

macOS 10.4–10.12Deprecated

``` source
func setMaximumLength(_ maxLen: Int)
```

## Parameters 

`maxLen`  

The maximum number of characters allowed in the annotation string. Pass `0` to indicate that there is no specified maximum.

## See Also

### Related Documentation

class PDFAnnotationTextWidget

A `PDFAnnotationTextWidget` object allows you to manage the appearance and content of text fields.

Deprecated

### Working with Annotation Strings

func stringValue() -> String!

Returns the string assigned to the annotation.

Deprecated

func setStringValue(String!)

Sets the string for the annotation.

Deprecated

func maximumLength() -> Int

Returns the maximum number of characters allowed in the annotation string.

Deprecated

