

- Core Foundation
-  CFBundleCopyPreferredLocalizationsFromArray(\_:) 

Function

# CFBundleCopyPreferredLocalizationsFromArray(\_:)

Given an array of possible localizations, returns the one or more of them that CFBundle would use in the current application context.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyPreferredLocalizationsFromArray(_ locArray: CFArray!) -> CFArray!
```

## Parameters 

`locArray`  

An array of possible localizations.

## Return Value

A subset of `locArray` that CFBundle would use in the current application context. Ownership follows the The Create Rule.

## Discussion

You can obtain `locArray` using the CFBundleCopyBundleLocalizations(_:) function.

## See Also

### Managing Localizations

func CFBundleCopyBundleLocalizations(CFBundle!) -> CFArray!

Returns an array containing a bundle’s localizations.

func CFBundleCopyLocalizedString(CFBundle!, CFString!, CFString!, CFString!) -> CFString!

Returns a localized string from a bundle’s strings file.

func CFBundleCopyLocalizationsForPreferences(CFArray!, CFArray!) -> CFArray!

Given an array of possible localizations and preferred locations, returns the one or more of them that CFBundle would use, without reference to the current application context.

func CFBundleCopyLocalizationsForURL(CFURL!) -> CFArray!

Returns an array containing the localizations for a bundle or executable at a particular location.

