

- Foundation
- NSAttributedString
- NSAttributedString.DocumentReadingOptionKey
-  textSizeMultiplier 

Type Property

# textSizeMultiplier

The scale factor for font sizes.

FoundationAppKitmacOS 10.0+

``` source
static let textSizeMultiplier: NSAttributedString.DocumentReadingOptionKey
```

## Discussion

NSNumber containing float, default 1.0; for HTML only, corresponding to WebView’s `textSizeMultiplier`.

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

static let timeout: NSAttributedString.DocumentReadingOptionKey

The time, in seconds, to wait for a document to finish loading.

static let webPreferences: NSAttributedString.DocumentReadingOptionKey

A WebPreferences object.

static let webResourceLoadDelegate: NSAttributedString.DocumentReadingOptionKey

An object to serve as the web resource loading delegate.

