

- PDFKit
- PDFAnnotationStamp
-  name() Deprecated

Instance Method

# name()

Returns name associated with the stamp annotation.

macOS 10.5–10.12Deprecated

``` source
func name() -> String!
```

## Discussion

Note that the name value of the stamp annotation is not necessarily identical to the user-visible appearance of the stamp annotation. For example, a stamp annotation that displays “Confidential” on a PDF page may not have a name value of “Confidential”.

## See Also

### Accessing and setting the stamp annotation

func setName(String!)

Sets the name associated with the stamp annotation.

Deprecated

