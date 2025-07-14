

- Core Graphics
- CGFont
-  table(for:) 

Instance Method

# table(for:)

Returns the font table that corresponds to the provided tag.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func table(for tag: UInt32) -> CFData?
```

## Parameters 

`tag`  

The tag for the table you want to obtain.

## Return Value

The font table that corresponds to the tag, or `nil` if no such table exists.

## See Also

### Working with Font Tables

var tableTags: CFArray?

Returns an array of tags that correspond to the font tables for a font.

Font Table Index Values

Possible values for an index into a font table.

Obsolete Font Table Index Values

Deprecated values for an index into a font table.

