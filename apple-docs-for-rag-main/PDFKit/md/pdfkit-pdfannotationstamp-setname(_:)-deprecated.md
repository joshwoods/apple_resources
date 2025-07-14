

- PDFKit
- PDFAnnotationStamp
-  setName(\_:) Deprecated

Instance Method

# setName(\_:)

Sets the name associated with the stamp annotation.

macOS 10.5–10.12Deprecated

``` source
func setName(_ name: String!)
```

## Discussion

The name must be representable in ASCII. You can set a stamp annotation’s name to help you identify it, but that name is not displayed on the PDF page. You must provide the string you want displayed on the page, such as “Draft” or “Top Secret”, in the appearance stream for the annotation.

## See Also

### Accessing and setting the stamp annotation

func name() -> String!

Returns name associated with the stamp annotation.

Deprecated

