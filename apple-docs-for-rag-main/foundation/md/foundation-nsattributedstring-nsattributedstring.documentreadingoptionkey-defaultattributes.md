

- Foundation
- NSAttributedString
- NSAttributedString.DocumentReadingOptionKey
-  defaultAttributes 

Type Property

# defaultAttributes

The default attributes to apply to plain files.

FoundationUIKitiOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let defaultAttributes: NSAttributedString.DocumentReadingOptionKey
```

## Discussion

For plain text documents; NSDictionary containing attributes to be applied to plain files. The previous string constant was `@"DefaultAttributes"`.

## See Also

### Getting the document options

static let baseURL: NSAttributedString.DocumentReadingOptionKey

The base URL for HTML documents.

static let characterEncoding: NSAttributedString.DocumentReadingOptionKey

The string encoding.

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

static let timeout: NSAttributedString.DocumentReadingOptionKey

The time, in seconds, to wait for a document to finish loading.

static let webPreferences: NSAttributedString.DocumentReadingOptionKey

A WebPreferences object.

static let webResourceLoadDelegate: NSAttributedString.DocumentReadingOptionKey

An object to serve as the web resource loading delegate.

