

- Core Foundation
-  CFStringHasPrefix(\_:\_:) 

Function

# CFStringHasPrefix(\_:\_:)

Determines if the character data of a string begin with a specified sequence of characters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringHasPrefix(
    _ theString: CFString!,
    _ prefix: CFString!
) -> Bool
```

## Parameters 

`theString`  

The string to search.

`prefix`  

The prefix to search for.

## Return Value

`true` if `theString` begins with `prefix`, `false` if otherwise.

## See Also

### Comparing Strings

func CFStringCompare(CFString!, CFString!, CFStringCompareFlags) -> CFComparisonResult

Compares one string with another string.

func CFStringCompareWithOptions(CFString!, CFString!, CFRange, CFStringCompareFlags) -> CFComparisonResult

Compares a range of the characters in one string with that of another string.

func CFStringCompareWithOptionsAndLocale(CFString!, CFString!, CFRange, CFStringCompareFlags, CFLocale!) -> CFComparisonResult

Compares a range of the characters in one string with another string using a given locale.

func CFStringHasSuffix(CFString!, CFString!) -> Bool

Determines if a string ends with a specified sequence of characters.

