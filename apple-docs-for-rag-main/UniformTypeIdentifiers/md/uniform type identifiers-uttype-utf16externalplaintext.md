

- Uniform Type Identifiers
- UTType
-  utf16ExternalPlainText 

Type Property

# utf16ExternalPlainText

A type that represents plain text encoded as UTF-16 with an optional bill of materials.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var utf16ExternalPlainText: UTType { get }
```

## Discussion

If the bill of materials isn’t present, the encoding uses “external byte order (big-endian),

The identifier for this type is `public.utf16-external-plain-text`.

This type conforms to UTTypePlainText.

## See Also

### Text files

static var text: UTType

A base type that represents all text-encoded data, including text with markup.

static var plainText: UTType

A type that represents text with no markup and an unspecified encoding.

static var utf8PlainText: UTType

A type that represents plain text encoded as UTF-8.

static var utf16PlainText: UTType

A type that represents plain text encoded as UTF-16 in native byte order with an optional bill of materials.

