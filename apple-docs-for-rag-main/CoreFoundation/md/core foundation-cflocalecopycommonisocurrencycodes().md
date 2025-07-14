

- Core Foundation
-  CFLocaleCopyCommonISOCurrencyCodes() 

Function

# CFLocaleCopyCommonISOCurrencyCodes()

Returns an array of strings that represents ISO currency codes for currencies in common use.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFLocaleCopyCommonISOCurrencyCodes() -> CFArray!
```

## Return Value

An array of CFString objects that represents ISO currency codes for currencies in common use. Ownership follows the The Create Rule.

## See Also

### Getting ISO Information

func CFLocaleCopyISOCountryCodes() -> CFArray!

Returns an array of CFString objects that represents all known legal ISO country codes.

func CFLocaleCopyISOLanguageCodes() -> CFArray!

Returns an array of CFString objects that represents all known legal ISO language codes.

func CFLocaleCopyISOCurrencyCodes() -> CFArray!

Returns an array of CFString objects that represents all known legal ISO currency codes.

