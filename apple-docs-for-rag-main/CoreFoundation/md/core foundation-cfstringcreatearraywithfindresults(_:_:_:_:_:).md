

- Core Foundation
-  CFStringCreateArrayWithFindResults(\_:\_:\_:\_:\_:) 

Function

# CFStringCreateArrayWithFindResults(\_:\_:\_:\_:\_:)

Searches a string for multiple occurrences of a substring and creates an array of ranges identifying the locations of these substrings within the target string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringCreateArrayWithFindResults(
    _ alloc: CFAllocator!,
    _ theString: CFString!,
    _ stringToFind: CFString!,
    _ rangeToSearch: CFRange,
    _ compareOptions: CFStringCompareFlags
) -> CFArray!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new CFArray object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theString`  

The string in which to search for `stringToFind`.

`stringToFind`  

The string to search for in `theString`.

`rangeToSearch`  

The range of characters within `theString` to be searched. The specified range must not exceed the length of the string.

`compareOptions`  

Flags that select different types of comparisons, such as localized comparison, case-insensitive comparison, and non-literal comparison. If you want the default comparison behavior, pass `0`. See String Comparison Flags for the available flags.

## Return Value

An array that contains pointers to CFRange structures identifying the character locations of `stringToFind` in `theString`. Returns `NULL`, if no matching substring is found in the source object, or if there was a problem creating the array. Ownership follows the The Create Rule.

## See Also

### Searching Strings

func CFStringFind(CFString!, CFString!, CFStringCompareFlags) -> CFRange

Searches for a substring within a string and, if it is found, yields the range of the substring within the object’s characters.

func CFStringFindCharacterFromSet(CFString!, CFCharacterSet!, CFRange, CFStringCompareFlags, UnsafeMutablePointer&lt;CFRange>!) -> Bool

Query the range of the first character contained in the specified character set.

func CFStringFindWithOptions(CFString!, CFString!, CFRange, CFStringCompareFlags, UnsafeMutablePointer&lt;CFRange>!) -> Bool

Searches for a substring within a range of the characters represented by a string and, if the substring is found, returns its range within the object’s characters.

func CFStringFindWithOptionsAndLocale(CFString!, CFString!, CFRange, CFStringCompareFlags, CFLocale!, UnsafeMutablePointer&lt;CFRange>!) -> Bool

Returns a Boolean value that indicates whether a given string was found in a given source string.

func CFStringGetLineBounds(CFString!, CFRange, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!, UnsafeMutablePointer&lt;CFIndex>!)

Given a range of characters in a string, obtains the line bounds—that is, the indexes of the first character and the final characters of the lines containing the range.

