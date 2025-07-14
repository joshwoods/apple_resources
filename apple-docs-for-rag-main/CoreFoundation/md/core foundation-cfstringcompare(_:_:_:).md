

- Core Foundation
-  CFStringCompare(\_:\_:\_:) 

Function

# CFStringCompare(\_:\_:\_:)

Compares one string with another string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringCompare(
    _ theString1: CFString!,
    _ theString2: CFString!,
    _ compareOptions: CFStringCompareFlags
) -> CFComparisonResult
```

## Parameters 

`theString1`  

The first string to use in the comparison.

`theString2`  

The second string to use in the comparison.

`compareOptions`  

Flags that select different types of comparisons, such as localized comparison, case-insensitive comparison, and non-literal comparison. If you want the default comparison behavior, pass `0`. See String Comparison Flags for the available flags.

## Return Value

A CFComparisonResult value that indicates whether `theString1` is equal to, less than, or greater than `theString2`.

## Discussion

You can affect how the comparison proceeds by specifying one or more option flags in `compareOptions`. Not all comparison options are currently implemented.

## See Also

### Comparing Strings

func CFStringCompareWithOptions(CFString!, CFString!, CFRange, CFStringCompareFlags) -> CFComparisonResult

Compares a range of the characters in one string with that of another string.

func CFStringCompareWithOptionsAndLocale(CFString!, CFString!, CFRange, CFStringCompareFlags, CFLocale!) -> CFComparisonResult

Compares a range of the characters in one string with another string using a given locale.

func CFStringHasPrefix(CFString!, CFString!) -> Bool

Determines if the character data of a string begin with a specified sequence of characters.

func CFStringHasSuffix(CFString!, CFString!) -> Bool

Determines if a string ends with a specified sequence of characters.

