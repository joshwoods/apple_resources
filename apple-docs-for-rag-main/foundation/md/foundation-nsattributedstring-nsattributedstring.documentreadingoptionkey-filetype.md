

- Foundation
- NSAttributedString
- NSAttributedString.DocumentReadingOptionKey
-  fileType 

Type Property

# fileType

The file type.

FoundationAppKitmacOS 10.6+

``` source
static let fileType: NSAttributedString.DocumentReadingOptionKey
```

## Discussion

The value of this attribute is an NSString object indicating a document type to be forced when loading the document, specified as a UTI string; mutually exclusive with documentType.

## See Also

### Getting the document options

static let baseURL: NSAttributedString.DocumentReadingOptionKey

The base URL for HTML documents.

static let characterEncoding: NSAttributedString.DocumentReadingOptionKey

The string encoding.

static let defaultAttributes: NSAttributedString.DocumentReadingOptionKey

The default attributes to apply to plain files.

static let documentType: NSAttributedString.DocumentReadingOptionKey

The document type.

static let readAccessURL: NSAttributedString.DocumentReadingOptionKey

The local files WebKit can access when loading content.

static let textEncodingName: NSAttributedString.DocumentReadingOptionKey

The text encoding to use.

static let textSizeMultiplier: NSAttributedString.DocumentReadingOptionKey

The scale factor for font sizes.

static let timeout: NSAttributedString.DocumentReadingOptionKey

The time, in seconds, to wait for a document to finish loading.

static let webPreferences: NSAttributedString.DocumentReadingOptionKey

A WebPreferences object.

static let webResourceLoadDelegate: NSAttributedString.DocumentReadingOptionKey

An object to serve as the web resource loading delegate.

