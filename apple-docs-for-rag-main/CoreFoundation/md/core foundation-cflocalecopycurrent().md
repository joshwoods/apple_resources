

- Core Foundation
-  CFLocaleCopyCurrent() 

Function

# CFLocaleCopyCurrent()

Returns a copy of the logical locale for the current user.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFLocaleCopyCurrent() -> CFLocale!
```

## Return Value

The logical locale for the current user that is formed from the settings for the current user’s chosen system locale overlaid with any custom settings the user has specified in System Preferences. May return a retained cached object, not a new object. Ownership follows the The Create Rule.

## Discussion

Settings you get from this locale do not change as a user’s preferences are changed so that your operations are consistent. Typically you perform some operations on the returned object and then release it. Since the returned object may be cached, you do not need to hold on to it indefinitely.

Note that locale settings are independent of the user’s language setting. The language of the current locale may not correspond to the language at the first index in the `AppleLanguages` array from user defaults. For more details, see Locale Concepts in Locales Programming Guide; see also CFLocaleCopyPreferredLanguages().

## See Also

### Creating a Locale

func CFLocaleCreate(CFAllocator!, CFLocaleIdentifier!) -> CFLocale!

Creates a locale for the given arbitrary locale identifier.

func CFLocaleCreateCopy(CFAllocator!, CFLocale!) -> CFLocale!

Returns a copy of a locale.

func CFLocaleGetSystem() -> CFLocale!

Returns the root, canonical locale.

