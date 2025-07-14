

- Core Services
- Dictionary Services
-  DCSGetTermRangeInString(\_:\_:\_:) 

Function

# DCSGetTermRangeInString(\_:\_:\_:)

Determines the range of the longest word or phrase with respect to an offset.

Mac Catalyst 13.1+macOS 10.5+

``` source
func DCSGetTermRangeInString(
    _ dictionary: DCSDictionary?,
    _ textString: CFString,
    _ offset: CFIndex
) -> CFRange
```

## Parameters 

`dictionary`  

This parameter is reserved for future use, so pass `NULL`. Dictionary Services searches in all active dictionaries.

`textString`  

Text that contains the word or phrase to look up.

`offset`  

A character offset in the `textString` parameter.

## Return Value

The range that specifies the location, around the specified offset, of the word or phrase , or the constant `kCFNotFound`.

## Discussion

You can use this function to determine the range of text that contains a word or phrase. After you determine the range, you can pass the result to the functions DCSCopyTextDefinition(_:_:_:) and `HIDictionaryWindowShow(_:_:_:_:_:_:_:)`.

To see how this works, follow these steps:

1.  In macOS 10.5 or later, open Text Edit.

2.  Type `It is a foggy day in San Francisco, California.`

3.  Control-click `Francisco` (don’t select it). Then, choose “Lookup in Dictionary”.

Note that the Dictionary window appears with a definition of San Francisco. The function `DCSGetTermRangeInString` automatically detected the range of the phrase San Francisco, using `Francisco` as the text string to search for and a character offset in this string. The function expanded the range until it found a possible match.

You can also point the cursor at the word `Francisco` and, without making a selection or clicking, type Command-Control-D. `DCSGetTermRangeInString` detects the range.

The function `DCSGetTermRangeInString` only returns the range. You must call DCSCopyTextDefinition(_:_:_:) to copy the definition and `HIDictionaryWindowShow(_:_:_:_:_:_:_:)` to display the definition in a Dictionary window.

## See Also

### Related Documentation

Dictionary Services Programming Guide

