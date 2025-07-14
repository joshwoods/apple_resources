

- Foundation
- NSAttributedString
- NSAttributedString.DocumentReadingOptionKey
-  characterEncoding 

Type Property

# characterEncoding

The string encoding.

FoundationUIKitiOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let characterEncoding: NSAttributedString.DocumentReadingOptionKey
```

## Discussion

For plain text documents; NSNumber containing the unsigned int NSStringEncoding to override any encoding specified in an HTML document. The previous string constant was `@"CharacterEncoding"`.

## See Also

### Getting the document options

static let baseURL: NSAttributedString.DocumentReadingOptionKey

The base URL for HTML documents.

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

static let timeout: NSAttributedString.DocumentReadingOptionKey

The time, in seconds, to wait for a document to finish loading.

static let webPreferences: NSAttributedString.DocumentReadingOptionKey

A WebPreferences object.

static let webResourceLoadDelegate: NSAttributedString.DocumentReadingOptionKey

An object to serve as the web resource loading delegate.

