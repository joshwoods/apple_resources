

- Foundation
- ByteCountFormatStyle
-  ByteCountFormatStyle.Style 

Enumeration

# ByteCountFormatStyle.Style

The semantic style to use when formatting a byte count value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Style
```

## Topics

### Byte count styles

case binary

A style for representing byte counts as binary values.

case decimal

A style for representing byte counts as decimal values.

case file

A style for representing file system storage.

case memory

The style for representing memory usage.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing style behavior

var style: ByteCountFormatStyle.Style

The semantic style the format style uses to represent a byte count value.

