

- Foundation
- NSAttributedString
- NSAttributedString.DocumentAttributeKey
-  fileType 

Type Property

# fileType

The document type for interpreting the document.

FoundationAppKitmacOS 10.6+

``` source
static let fileType: NSAttributedString.DocumentAttributeKey
```

## Discussion

The value of this attribute is an NSString object indicating which document type was used to interpret the document, specified as a UTI; for reading, this is available along with documentType, but for writing the two are mutually exclusive.

## See Also

### Getting document type keys

static let documentType: NSAttributedString.DocumentAttributeKey

The document type.

static let textEncodingName: NSAttributedString.DocumentAttributeKey

The name of the text encoding to use.

