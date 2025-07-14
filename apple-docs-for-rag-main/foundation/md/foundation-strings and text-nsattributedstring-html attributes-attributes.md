

- Foundation
- Strings and Text
- NSAttributedString
-  HTML attributes 

API Collection

# HTML attributes

Documentwide attributes that provide control over the form of generated HTML.

## Overview

You use these attributes only for writing HTML. excludedElements allows control over the tags used. The recognized values in the excludedElements array are (case-insensitive) HTML tags, plus DOCTYPE (representing a doctype declaration) and XML (representing an XML declaration). By default, if this attribute is not present, the excluded elements will be those deprecated in HTML 4 (APPLET, BASEFONT, CENTER, DIR, FONT, ISINDEX, MENU, S, STRIKE, and U) plus XML. If XML is on the list, HTML forms are used; if XML is not on the list, XHTML forms are used where there is a distinction. Either characterEncoding or textEncodingName may be used to control the encoding used for generated HTML; character entities are used for characters not representable in the specified encoding. prefixSpaces allows some control over formatting.

## Topics

### Getting the attributes

static let excludedElements: NSAttributedString.DocumentAttributeKey

The HTML elements to exclude in generated HTML.

static let textEncodingName: NSAttributedString.DocumentAttributeKey

The name of the text encoding to use.

static let prefixSpaces: NSAttributedString.DocumentAttributeKey

The number of spaces for indenting nested HTML elements.

## See Also

### Getting document-wide attributes

struct DocumentAttributeKey

The attributes you apply to an entire document.

struct DocumentReadingOptionKey

Options for constructing an attributed string from data you read from disk.

struct DocumentType

Constants for the document type document attribute key.

struct TextLayoutSectionKey

Constants for the text layout sections document attribute key.

enum NSTextScalingType

Constants that specify the text scaling.

