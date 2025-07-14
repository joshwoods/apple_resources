

- Foundation
- NSAttributedString
-  NSAttributedString.DocumentReadingOptionKey 

Structure

# NSAttributedString.DocumentReadingOptionKey

Options for constructing an attributed string from data you read from disk.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct DocumentReadingOptionKey
```

## Overview

The NSAttributedString.DocumentReadingOptionKey type defines attributes to use when creating an attributed string from data in a file. Use these strings with methods such as init(data:options:documentAttributes:), init(HTML:options:documentAttributes:), init(URL:options:documentAttributes:), read(from:options:documentAttributes:), and read(from:options:documentAttributes:) to specify expected details. For example, specify the documentType attribute to interpret the file data as a specific file format.

## Topics

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

static let timeout: NSAttributedString.DocumentReadingOptionKey

The time, in seconds, to wait for a document to finish loading.

static let webPreferences: NSAttributedString.DocumentReadingOptionKey

A WebPreferences object.

static let webResourceLoadDelegate: NSAttributedString.DocumentReadingOptionKey

An object to serve as the web resource loading delegate.

### Getting the font-scaling options

static let sourceTextScaling: NSAttributedString.DocumentReadingOptionKey

The text-scaling mode to associate with the document’s content.

static let targetTextScaling: NSAttributedString.DocumentReadingOptionKey

The text scaling mode to use after reading the text from disk.

### Initializers

init(String)

Creates a document reading option key with the specified raw value.

init(rawValue: String)

### Type Properties

static let textKit1ListMarkerFormatDocumentOption: NSAttributedString.DocumentReadingOptionKey

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting document-wide attributes

struct DocumentAttributeKey

The attributes you apply to an entire document.

HTML attributes

Documentwide attributes that provide control over the form of generated HTML.

struct DocumentType

Constants for the document type document attribute key.

struct TextLayoutSectionKey

Constants for the text layout sections document attribute key.

enum NSTextScalingType

Constants that specify the text scaling.

