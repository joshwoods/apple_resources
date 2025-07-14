

- Core Graphics
- CGFont
-  tableTags 

Instance Property

# tableTags

Returns an array of tags that correspond to the font tables for a font.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var tableTags: CFArray? { get }
```

## Discussion

Each entry in the returned array is a four-byte value that represents a single TrueType or OpenType font table tag. To obtain a tag at index `k` in a manner that is appropriate for 32-bit and 64-bit architectures, you need to use code similar to the following:

```
```

## See Also

### Working with Font Tables

func table(for: UInt32) -> CFData?

Returns the font table that corresponds to the provided tag.

Font Table Index Values

Possible values for an index into a font table.

Obsolete Font Table Index Values

Deprecated values for an index into a font table.

