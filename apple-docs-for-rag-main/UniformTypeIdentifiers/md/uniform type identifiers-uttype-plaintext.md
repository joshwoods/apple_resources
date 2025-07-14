

- Uniform Type Identifiers
- UTType
-  plainText 

Type Property

# plainText

A type that represents text with no markup and an unspecified encoding.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var plainText: UTType { get }
```

## Discussion

The identifier for this type is `public.plain-text`.

This type conforms to UTTypeText.

## See Also

### Text files

static var text: UTType

A base type that represents all text-encoded data, including text with markup.

static var utf8PlainText: UTType

A type that represents plain text encoded as UTF-8.

static var utf16PlainText: UTType

A type that represents plain text encoded as UTF-16 in native byte order with an optional bill of materials.

static var utf16ExternalPlainText: UTType

A type that represents plain text encoded as UTF-16 with an optional bill of materials.

