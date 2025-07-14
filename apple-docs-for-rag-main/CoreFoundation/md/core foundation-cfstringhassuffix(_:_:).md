

- Core Foundation
-  CFStringHasSuffix(\_:\_:) 

Function

# CFStringHasSuffix(\_:\_:)

Determines if a string ends with a specified sequence of characters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFStringHasSuffix(
    _ theString: CFString!,
    _ suffix: CFString!
) -> Bool
```

## Parameters 

`theString`  

The string to be evaluated.

`suffix`  

The suffix to search for.

## Return Value

`true` if `theString` ends with `suffix`, `false` otherwise.

## See Also

### Comparing Strings

func CFStringCompare(CFString!, CFString!, CFStringCompareFlags) -> CFComparisonResult

Compares one string with another string.

func CFStringCompareWithOptions(CFString!, CFString!, CFRange, CFStringCompareFlags) -> CFComparisonResult

Compares a range of the characters in one string with that of another string.

func CFStringCompareWithOptionsAndLocale(CFString!, CFString!, CFRange, CFStringCompareFlags, CFLocale!) -> CFComparisonResult

Compares a range of the characters in one string with another string using a given locale.

func CFStringHasPrefix(CFString!, CFString!) -> Bool

Determines if the character data of a string begin with a specified sequence of characters.

