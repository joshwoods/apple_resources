

- Foundation
- NSAttributedString
-  NSAttributedString.DocumentType 

Structure

# NSAttributedString.DocumentType

Constants for the document type document attribute key.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct DocumentType
```

## Overview

Use these constants as values for the documentType key in the document attributes dictionary.

## Topics

### Getting keys for document types

static let docFormat: NSAttributedString.DocumentType

Microsoft Word document.

static let html: NSAttributedString.DocumentType

Hypertext markup language (HTML) document.

static let macSimpleText: NSAttributedString.DocumentType

Macintosh SimpleText document.

static let officeOpenXML: NSAttributedString.DocumentType

ECMA Office Open XML text document format.

static let openDocument: NSAttributedString.DocumentType

OASIS Open Document text document format.

static let plain: NSAttributedString.DocumentType

Plain text document.

static let rtf: NSAttributedString.DocumentType

Rich text format document.

static let rtfd: NSAttributedString.DocumentType

Rich text format with attachments document.

static let webArchive: NSAttributedString.DocumentType

WebKit WebArchive document.

static let wordML: NSAttributedString.DocumentType

Microsoft Word XML (WordML schema) document.

### Initializers

init(String)

Creates a document type.

init(rawValue: String)

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

struct DocumentReadingOptionKey

Options for constructing an attributed string from data you read from disk.

HTML attributes

Documentwide attributes that provide control over the form of generated HTML.

struct TextLayoutSectionKey

Constants for the text layout sections document attribute key.

enum NSTextScalingType

Constants that specify the text scaling.

