

- Uniform Type Identifiers
- UTType
-  utf8TabSeparatedText 

Type Property

# utf8TabSeparatedText

A type that represents UTF-8–encoded text containing tab-separated values.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var utf8TabSeparatedText: UTType { get }
```

## Discussion

The identifier for this type is `public.utf8-tab-separated-values-text`.

This type conforms to UTTypeDelimitedText and UTTypeUTF8PlainText.

## See Also

### Data interchange formats

static var delimitedText: UTType

A base type that represents text containing delimited values.

static var commaSeparatedText: UTType

A type that represents text containing comma-separated values.

static var tabSeparatedText: UTType

A type that represents text containing tab-separated values.

static var rtf: UTType

A type that represents Rich Text Format data.

static var xml: UTType

A type that represents generic XML data.

static var yaml: UTType

A type that represents Yet Another Markup Language data.

static var json: UTType

A type that represents JavaScript Object Notation (JSON) data.

static var vCard: UTType

A type that represents a vCard file.

