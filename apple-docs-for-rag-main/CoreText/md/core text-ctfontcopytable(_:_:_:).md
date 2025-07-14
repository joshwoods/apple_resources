

- Core Text
-  CTFontCopyTable(\_:\_:\_:) 

Function

# CTFontCopyTable(\_:\_:\_:)

Returns a reference to the font table data.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontCopyTable(
    _ font: CTFont,
    _ table: CTFontTableTag,
    _ options: CTFontTableOptions
) -> CFData?
```

## Parameters 

`font`  

The font reference.

`table`  

The font table identifier as a CTFontTableTag constant. See CTFontTableTag for possible values.

`options`  

The font table options.

## Return Value

A retained reference to the font table data as a CFData object. The table data is not actually copied; however, the data reference must be released.

## See Also

### Getting Font Table Data

func CTFontCopyAvailableTables(CTFont, CTFontTableOptions) -> CFArray?

Returns an array of font table tags.

