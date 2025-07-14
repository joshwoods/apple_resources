

- Core Foundation
-  CFLocaleCopyISOCurrencyCodes() 

Function

# CFLocaleCopyISOCurrencyCodes()

Returns an array of CFString objects that represents all known legal ISO currency codes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFLocaleCopyISOCurrencyCodes() -> CFArray!
```

## Return Value

An array of CFString objects that represents all known legal ISO currency codes.Ownership follows the The Create Rule.

## Discussion

Note: many of these will not have any supporting locale data in macOS.

## See Also

### Getting ISO Information

func CFLocaleCopyISOCountryCodes() -> CFArray!

Returns an array of CFString objects that represents all known legal ISO country codes.

func CFLocaleCopyISOLanguageCodes() -> CFArray!

Returns an array of CFString objects that represents all known legal ISO language codes.

func CFLocaleCopyCommonISOCurrencyCodes() -> CFArray!

Returns an array of strings that represents ISO currency codes for currencies in common use.

