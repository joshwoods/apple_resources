

- Foundation
- NSAttributedString
-  NSAttributedString.DocumentAttributeKey 

Structure

# NSAttributedString.DocumentAttributeKey

The attributes you apply to an entire document.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct DocumentAttributeKey
```

## Overview

The NSAttributedString.DocumentAttributeKey type defines attributes that apply to an entire attributed string, and not to specific ranges of characters. You specify these attributes when writing an attributed string to disk, or reading text from a file on disk. Use these attributes to specify metadata about the overall document, including its author or title, page margin details, font-scaling options for cross-platform interchange, and more.

## Topics

### Getting document type keys

static let documentType: NSAttributedString.DocumentAttributeKey

The document type.

static let fileType: NSAttributedString.DocumentAttributeKey

The document type for interpreting the document.

static let textEncodingName: NSAttributedString.DocumentAttributeKey

The name of the text encoding to use.

### Getting document metadata keys

static let author: NSAttributedString.DocumentAttributeKey

The author of the document.

static let category: NSAttributedString.DocumentAttributeKey

The document’s category.

static let characterEncoding: NSAttributedString.DocumentAttributeKey

The string encoding for the document.

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

### Getting document appearance keys

static let appearance: NSAttributedString.DocumentAttributeKey

The appearance of the document.

static let backgroundColor: NSAttributedString.DocumentAttributeKey

The background color of the document.

static let bottomMargin: NSAttributedString.DocumentAttributeKey

The bottom margin of the document.

static let defaultFontExcluded: NSAttributedString.DocumentAttributeKey

static let defaultTabInterval: NSAttributedString.DocumentAttributeKey

The default tab stop interval for the document.

static let excludedElements: NSAttributedString.DocumentAttributeKey

The HTML elements to exclude in generated HTML.

static let hyphenationFactor: NSAttributedString.DocumentAttributeKey

The hyphenation factor of the document.

static let leftMargin: NSAttributedString.DocumentAttributeKey

The left margin of the document.

static let paperMargin: NSAttributedString.DocumentAttributeKey

The paper margin of the document.

static let paperSize: NSAttributedString.DocumentAttributeKey

The paper size for the document.

static let prefixSpaces: NSAttributedString.DocumentAttributeKey

The number of spaces for indenting nested HTML elements.

static let rightMargin: NSAttributedString.DocumentAttributeKey

The right margin of the document.

static let textLayoutSections: NSAttributedString.DocumentAttributeKey

The layout orientations for each section.

static let topMargin: NSAttributedString.DocumentAttributeKey

The top margin of the document.

static let viewMode: NSAttributedString.DocumentAttributeKey

The view mode.

static let viewSize: NSAttributedString.DocumentAttributeKey

The view size.

static let viewZoom: NSAttributedString.DocumentAttributeKey

The view zoom.

### Getting the font-scaling options

static let sourceTextScaling: NSAttributedString.DocumentAttributeKey

The text-scaling mode you used when creating the text.

static let textScaling: NSAttributedString.DocumentAttributeKey

The text-scaling mode to use when displaying the text.

### Getting the default attributes

static let defaultAttributes: NSAttributedString.DocumentAttributeKey

The default document attributes.

### Initializers

init(String)

Creates a document attribute key.

init(rawValue: String)

### Type Properties

static let cocoaVersionDocumentAttribute: NSAttributedString.DocumentAttributeKey

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting document-wide attributes

struct DocumentReadingOptionKey

Options for constructing an attributed string from data you read from disk.

HTML attributes

Documentwide attributes that provide control over the form of generated HTML.

struct DocumentType

Constants for the document type document attribute key.

struct TextLayoutSectionKey

Constants for the text layout sections document attribute key.

enum NSTextScalingType

Constants that specify the text scaling.

