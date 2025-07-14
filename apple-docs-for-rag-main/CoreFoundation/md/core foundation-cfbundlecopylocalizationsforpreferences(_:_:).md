

- Core Foundation
-  CFBundleCopyLocalizationsForPreferences(\_:\_:) 

Function

# CFBundleCopyLocalizationsForPreferences(\_:\_:)

Given an array of possible localizations and preferred locations, returns the one or more of them that CFBundle would use, without reference to the current application context.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyLocalizationsForPreferences(
    _ locArray: CFArray!,
    _ prefArray: CFArray!
) -> CFArray!
```

## Parameters 

`locArray`  

An array of possible localizations to search.

`prefArray`  

An array of preferred localizations. If `NULL`, the user’s actual preferred localizations will be used.

## Return Value

An array containing the localizations that CFBundle would use. Ownership follows the The Create Rule.

## Discussion

This is not the same as CFBundleCopyPreferredLocalizationsFromArray(_:), because that function takes the current application context into account. To determine the localizations that another application would use, apply this function to the result of CFBundleCopyBundleLocalizations(_:).

## See Also

### Managing Localizations

func CFBundleCopyBundleLocalizations(CFBundle!) -> CFArray!

Returns an array containing a bundle’s localizations.

func CFBundleCopyLocalizedString(CFBundle!, CFString!, CFString!, CFString!) -> CFString!

Returns a localized string from a bundle’s strings file.

func CFBundleCopyLocalizationsForURL(CFURL!) -> CFArray!

Returns an array containing the localizations for a bundle or executable at a particular location.

func CFBundleCopyPreferredLocalizationsFromArray(CFArray!) -> CFArray!

Given an array of possible localizations, returns the one or more of them that CFBundle would use in the current application context.

