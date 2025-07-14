

- Core Foundation
-  CFBundleCopyBundleLocalizations(\_:) 

Function

# CFBundleCopyBundleLocalizations(\_:)

Returns an array containing a bundle’s localizations.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyBundleLocalizations(_ bundle: CFBundle!) -> CFArray!
```

## Parameters 

`bundle`  

The bundle to examine.

## Return Value

An array containing `bundle`’s localizations. Ownership follows the The Create Rule.

## Discussion

The array returned by this function is typically passed as a parameter to either the CFBundleCopyPreferredLocalizationsFromArray(_:) or CFBundleCopyLocalizationsForPreferences(_:_:) function.

## See Also

### Managing Localizations

func CFBundleCopyLocalizedString(CFBundle!, CFString!, CFString!, CFString!) -> CFString!

Returns a localized string from a bundle’s strings file.

func CFBundleCopyLocalizationsForPreferences(CFArray!, CFArray!) -> CFArray!

Given an array of possible localizations and preferred locations, returns the one or more of them that CFBundle would use, without reference to the current application context.

func CFBundleCopyLocalizationsForURL(CFURL!) -> CFArray!

Returns an array containing the localizations for a bundle or executable at a particular location.

func CFBundleCopyPreferredLocalizationsFromArray(CFArray!) -> CFArray!

Given an array of possible localizations, returns the one or more of them that CFBundle would use in the current application context.

