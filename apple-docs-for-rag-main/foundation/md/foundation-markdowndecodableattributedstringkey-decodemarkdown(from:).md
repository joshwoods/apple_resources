

- Foundation
- MarkdownDecodableAttributedStringKey
-  decodeMarkdown(from:) 

Type Method

# decodeMarkdown(from:)

Decodes a value from the provided decoder.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func decodeMarkdown(from decoder: any Decoder) throws -> Self.Value
```

**Required** Default implementation provided.

## Parameters 

`decoder`  

The decoder to read data from.

## Return Value

The decoded value.

## Discussion

This method throws an error if reading from the decoder fails, or if the data read is corrupted or otherwise invalid.

## Default Implementations

### MarkdownDecodableAttributedStringKey Implementations

static func decodeMarkdown(from: any Decoder) throws -> Self.Value

Decodes a value from the provided decoder, using a default implementation.

