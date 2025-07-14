

- Core Foundation
-  CFStringCompareWithOptions(\_:\_:\_:\_:) 

Function

# CFStringCompareWithOptions(\_:\_:\_:\_:)

Compares a range of the characters in one string with that of another string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringCompareWithOptions(
    _ theString1: CFString!,
    _ theString2: CFString!,
    _ rangeToCompare: CFRange,
    _ compareOptions: CFStringCompareFlags
) -> CFComparisonResult
```

## Parameters 

`theString1`  

The first string to use in the comparison.

`theString2`  

The second string to use in the comparison.

`rangeToCompare`  

The range of characters in `theString1` to be used in the comparison to `theString2`. To use the whole string, pass the range `CFRangeMake(0, CFStringGetLength(theString1))` or use CFStringCompare(_:_:_:). The specified range must not exceed the length of the string.

`compareOptions`  

Flags that select different types of comparisons, such as localized comparison, case-insensitive comparison, and non-literal comparison. If you want the default comparison behavior, pass `0`. See String Comparison Flags for the available flags.

## Return Value

A CFComparisonResult value that indicates whether `theString1` is equal to, less than, or greater than `theString2`.

## Discussion

You can affect how the comparison proceeds by specifying one or more option flags in `compareOptions`.

If you want to compare one entire string with another string, use the CFStringCompare(_:_:_:) function.

## See Also

### Comparing Strings

func CFStringCompare(CFString!, CFString!, CFStringCompareFlags) -> CFComparisonResult

Compares one string with another string.

func CFStringCompareWithOptionsAndLocale(CFString!, CFString!, CFRange, CFStringCompareFlags, CFLocale!) -> CFComparisonResult

Compares a range of the characters in one string with another string using a given locale.

func CFStringHasPrefix(CFString!, CFString!) -> Bool

Determines if the character data of a string begin with a specified sequence of characters.

func CFStringHasSuffix(CFString!, CFString!) -> Bool

Determines if a string ends with a specified sequence of characters.

