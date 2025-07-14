

- Core Foundation
-  CFStringFindWithOptionsAndLocale(\_:\_:\_:\_:\_:\_:) 

Function

# CFStringFindWithOptionsAndLocale(\_:\_:\_:\_:\_:\_:)

Returns a Boolean value that indicates whether a given string was found in a given source string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFStringFindWithOptionsAndLocale(
    _ theString: CFString!,
    _ stringToFind: CFString!,
    _ rangeToSearch: CFRange,
    _ searchOptions: CFStringCompareFlags,
    _ locale: CFLocale!,
    _ result: UnsafeMutablePointer!
) -> Bool
```

## Parameters 

`theString`  

The string in which to to search for `stringToFind`.

`stringToFind`  

The substring to search for in `theString`.

`rangeToSearch`  

A range of the characters to search in `theString`. The specified range must not exceed the length of the string.

`searchOptions`  

The option flags to control the search behavior. See String Comparison Flags for possible values. The flags compareNumerically and compareForcedOrdering are ignored.

`locale`  

The locale to use for the search comparison. `NULL` specifies the canonical locale (the return value from CFLocaleGetSystem()).

The locale argument affects the equality checking algorithm. For example, for the Turkish locale, case-insensitive compare matches “I” to “ı” (Unicode code point U+0131, Latin Small Dotless I), not the normal “i” character.

`result`  

On return, if the function result is `true` contains the starting location and length of the found substring. You may pass `NULL` if you only want to know if the `theString` contains `stringToFind`.

## Return Value

`true` if the substring was found, `false` otherwise.

## Discussion

If `stringToFind` is the empty string (zero length), nothing is found.

## See Also

### Searching Strings

func CFStringCreateArrayWithFindResults(CFAllocator!, CFString!, CFString!, CFRange, CFStringCompareFlags) -> CFArray!

Searches a string for multiple occurrences of a substring and creates an array of ranges identifying the locations of these substrings within the target string.

func CFStringFind(CFString!, CFString!, CFStringCompareFlags) -> CFRange

Searches for a substring within a string and, if it is found, yields the range of the substring within the object’s characters.

func CFStringFindCharacterFromSet(CFString!, CFCharacterSet!, CFRange, CFStringCompareFlags, UnsafeMutablePointer&lt;CFRange>!) -> Bool

Query the range of the first character contained in the specified character set.

func CFStringFindWithOptions(CFString!, CFString!, CFRange, CFStringCompareFlags, UnsafeMutablePointer&lt;CFRange>!) -> Bool

Searches for a substring within a range of the characters represented by a string and, if the substring is found, returns its range within the object’s characters.

func CFStringGetLineBounds(CFString!, CFRange, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!)

Given a range of characters in a string, obtains the line bounds—that is, the indexes of the first character and the final characters of the lines containing the range.

