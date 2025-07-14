

- Core Foundation
-  CFBundleCopyLocalizationsForURL(\_:) 

Function

# CFBundleCopyLocalizationsForURL(\_:)

Returns an array containing the localizations for a bundle or executable at a particular location.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBundleCopyLocalizationsForURL(_ url: CFURL!) -> CFArray!
```

## Parameters 

`url`  

The location of a bundle’s localizations.

## Return Value

An array containing the localizations available at `url`. Ownership follows the The Create Rule.

## Discussion

For a directory URL, this is equivalent to calling the CFBundleCopyBundleLocalizations(_:) function on the corresponding bundle. For a plain file URL representing an unbundled application, this will attempt to determine its localizations using the kCFBundleLocalizationsKey and kCFBundleDevelopmentRegionKey keys in the dictionary returned by CFBundleCopyInfoDictionaryForURL(_:), or a `vers` resource if those are not present.

## See Also

### Managing Localizations

func CFBundleCopyBundleLocalizations(CFBundle!) -> CFArray!

Returns an array containing a bundle’s localizations.

func CFBundleCopyLocalizedString(CFBundle!, CFString!, CFString!, CFString!) -> CFString!

Returns a localized string from a bundle’s strings file.

func CFBundleCopyLocalizationsForPreferences(CFArray!, CFArray!) -> CFArray!

Given an array of possible localizations and preferred locations, returns the one or more of them that CFBundle would use, without reference to the current application context.

func CFBundleCopyPreferredLocalizationsFromArray(CFArray!) -> CFArray!

Given an array of possible localizations, returns the one or more of them that CFBundle would use in the current application context.

