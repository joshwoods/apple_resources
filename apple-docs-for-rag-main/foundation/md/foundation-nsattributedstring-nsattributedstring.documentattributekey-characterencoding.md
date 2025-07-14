

- Foundation
- NSAttributedString
- NSAttributedString.DocumentAttributeKey
-  characterEncoding 

Type Property

# characterEncoding

The string encoding for the document.

FoundationUIKitiOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let characterEncoding: NSAttributedString.DocumentAttributeKey
```

## Discussion

The value of this attribute is an NSNumber object containing integer specifying NSStringEncoding for the file; default for plain text is the default encoding. This key in options can specify the string encoding for reading the data. Upon return, the document attributes can contain the actual encoding used. For writing methods, this value is used for generating the plain text data.

The string constant in macOS 10.3 and earlier is `@"CharacterEncoding"`.

## See Also

### Getting document metadata keys

static let author: NSAttributedString.DocumentAttributeKey

The author of the document.

static let category: NSAttributedString.DocumentAttributeKey

The document’s category.

static let comment: NSAttributedString.DocumentAttributeKey

The document comments.

static let company: NSAttributedString.DocumentAttributeKey

The company or organization name associated with the document.

static let converted: NSAttributedString.DocumentAttributeKey

A value that indicates whether a filter service converted the file.

static let copyright: NSAttributedString.DocumentAttributeKey

The document’s copyright information.

static let creationTime: NSAttributedString.DocumentAttributeKey

The creation date of the document.

static let editor: NSAttributedString.DocumentAttributeKey

The name of person who last edited the document.

static let keywords: NSAttributedString.DocumentAttributeKey

The document keywords.

static let manager: NSAttributedString.DocumentAttributeKey

The name of the author’s manager.

static let modificationTime: NSAttributedString.DocumentAttributeKey

The modification date of the document.

static let readOnly: NSAttributedString.DocumentAttributeKey

An indication of whether the document is read-only.

static let subject: NSAttributedString.DocumentAttributeKey

The subject of the document.

static let title: NSAttributedString.DocumentAttributeKey

The document title.

