

- Foundation
- NSAttributedString
- NSAttributedString.DocumentReadingOptionKey
-  timeout 

Type Property

# timeout

The time, in seconds, to wait for a document to finish loading.

FoundationAppKitmacOS 10.0+

``` source
static let timeout: NSAttributedString.DocumentReadingOptionKey
```

## Discussion

The value is an NSNumber object containing a float. The previous string constant was `@"Timeout"`.

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

static let fileType: NSAttributedString.DocumentReadingOptionKey

The file type.

static let readAccessURL: NSAttributedString.DocumentReadingOptionKey

The local files WebKit can access when loading content.

static let textEncodingName: NSAttributedString.DocumentReadingOptionKey

The text encoding to use.

static let textSizeMultiplier: NSAttributedString.DocumentReadingOptionKey

The scale factor for font sizes.

static let webPreferences: NSAttributedString.DocumentReadingOptionKey

A WebPreferences object.

static let webResourceLoadDelegate: NSAttributedString.DocumentReadingOptionKey

An object to serve as the web resource loading delegate.

