

- Bundle Resources
- Information Property List
-  TICapsLockLanguageSwitchCapable 

Property List Key

# TICapsLockLanguageSwitchCapable

A Boolean value that enables the Caps Lock key to switch between Latin and non-Latin input sources.

macOS 10.15+

## Details 

Type  

boolean

## Discussion

Latin input sources, such as ABC, U.S., and Vietnamese, output characters in Latin script. Non-Latin input sources, such as Bulgarian (Cyrillic script), Hindi (Devanagari script), and Urdu (Arabic script), output characters in scripts other than Latin.

After implementing the key, users can enable or disable this functionality by modifying the “Use Caps Lock to switch to and from” preference, which can be found in System Preferences \> Keyboard \> Input Sources.

## See Also

### Localization

CFBundleDevelopmentRegion

The default language and region for the bundle, as a language ID.

**Name:** Localization native development region

CFBundleLocalizations

The localizations handled manually by your app.

**Name:** Localizations

CFBundleAllowMixedLocalizations

A Boolean value that indicates whether the bundle supports the retrieval of localized strings from frameworks.

**Name:** Localized resources can be mixed

