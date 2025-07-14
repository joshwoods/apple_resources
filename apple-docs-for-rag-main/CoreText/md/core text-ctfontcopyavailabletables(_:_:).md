

- Core Text
-  CTFontCopyAvailableTables(\_:\_:) 

Function

# CTFontCopyAvailableTables(\_:\_:)

Returns an array of font table tags.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyAvailableTables(
    _ font: CTFont,
    _ options: CTFontTableOptions
) -> CFArray?
```

## Parameters 

`font`  

The font reference.

`options`  

The font table options.

## Return Value

An array of CTFontTableTag values for the given font and the supplied options.

## Discussion

The returned set will contain unboxed values, which can be extracted like so:

```
```

## See Also

### Getting Font Table Data

func CTFontCopyTable(CTFont, CTFontTableTag, CTFontTableOptions) -> CFData?

Returns a reference to the font table data.

