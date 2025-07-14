

- Foundation
- NSAttributedString
- NSAttributedString.DocumentAttributeKey
-  documentType 

Type Property

# documentType

The document type.

FoundationUIKitiOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let documentType: NSAttributedString.DocumentAttributeKey
```

## Discussion

The value of this attribute is one of the document types declared in NSAttributedString.DocumentType. For reader methods, this key in options can specify the document type for interpreting the contents. Upon return, the document attributes can contain this key for indicating the actual format used to read the contents. For write methods, this key specifies the format for generating the data.

The string constant in macOS 10.3 and earlier is `@"DocumentType"`.

## See Also

### Getting document type keys

static let fileType: NSAttributedString.DocumentAttributeKey

The document type for interpreting the document.

static let textEncodingName: NSAttributedString.DocumentAttributeKey

The name of the text encoding to use.

