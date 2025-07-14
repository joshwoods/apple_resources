

- Foundation
- Strings and Text
- AttributedString
-  Encoding and Decoding Attributed String Keys 

API Collection

# Encoding and Decoding Attributed String Keys

Protocols adopted by attribute keys to encode or decode data.

## Topics

### Encoding and Decoding Keys

protocol DecodableAttributedStringKey

A protocol that defines how an attribute key decodes its value.

protocol EncodableAttributedStringKey

A protocol that defines how an attribute key encodes its value.

typealias CodableAttributedStringKey

A type alias used by attribute keys that are both encodable and decodable.

### Markdown Keys

protocol MarkdownDecodableAttributedStringKey

A protocol that defines how an attribute key decodes a value that corresponds to Markdown syntax.

## See Also

### Encoding and Decoding

struct AttributeScopeCodableConfiguration

A configuration type for encoding and decoding attributed strings.

