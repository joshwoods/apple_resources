

- Core Foundation
-  CFLocale 

Class

# CFLocale

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFLocale
```

## Overview

Unicode operations such as collation and text boundary determination can be affected by the conventions of a particular language or region. CFLocale objects specify language-specific or region-specific information for locale-sensitive operations.

The CFLocale opaque type provides support for obtaining available locales, obtaining localized locale names, and converting among locale data formats. Locale identifiers in macOS follow the IETF’s BCP 47. CFLocale never uses Script Manager codes (except for the legacy support provided by CFLocaleCreateCanonicalLocaleIdentifierFromScriptManagerCodes(_:_:_:))—the Script Manager and all its concepts are deprecated.

For more information on locale identifiers, read Internationalization and Localization Guide. It is also useful to read the ICU’s User Guide for the Locale Class.

CFLocale is “toll-free bridged” with its Cocoa Foundation counterpart, NSLocale. This means that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. Therefore, in a method where you see an `NSLocale *` parameter, you can pass in a `CFLocaleRef`, and in a function where you see a `CFLocaleRef` parameter, you can pass in an `NSLocale` instance. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

### Creating a Locale

func CFLocaleCopyCurrent() -> CFLocale!

Returns a copy of the logical locale for the current user.

func CFLocaleCreate(CFAllocator!, CFLocaleIdentifier!) -> CFLocale!

Creates a locale for the given arbitrary locale identifier.

func CFLocaleCreateCopy(CFAllocator!, CFLocale!) -> CFLocale!

Returns a copy of a locale.

func CFLocaleGetSystem() -> CFLocale!

Returns the root, canonical locale.

### Getting System Locale Information

func CFLocaleCopyAvailableLocaleIdentifiers() -> CFArray!

Returns an array of CFString objects that represents all locales for which locale data is available.

### Getting ISO Information

func CFLocaleCopyISOCountryCodes() -> CFArray!

Returns an array of CFString objects that represents all known legal ISO country codes.

func CFLocaleCopyISOLanguageCodes() -> CFArray!

Returns an array of CFString objects that represents all known legal ISO language codes.

func CFLocaleCopyISOCurrencyCodes() -> CFArray!

Returns an array of CFString objects that represents all known legal ISO currency codes.

func CFLocaleCopyCommonISOCurrencyCodes() -> CFArray!

Returns an array of strings that represents ISO currency codes for currencies in common use.

### Language Preferences

func CFLocaleCopyPreferredLanguages() -> CFArray!

Returns the array of canonicalized language IDs that the user prefers.

### Getting Information About a Locale

func CFLocaleCopyDisplayNameForPropertyValue(CFLocale!, CFLocaleKey!, CFString!) -> CFString!

Returns the display name for the given value.

func CFLocaleGetValue(CFLocale!, CFLocaleKey!) -> CFTypeRef!

Returns the corresponding value for the given key of a locale’s key-value pair.

func CFLocaleGetIdentifier(CFLocale!) -> CFLocaleIdentifier!

Returns the given locale’s identifier.

### Getting and Creating Locale Identifiers

func CFLocaleCreateCanonicalLocaleIdentifierFromScriptManagerCodes(CFAllocator!, LangCode, RegionCode) -> CFLocaleIdentifier!

Returns a canonical locale identifier from given language and region codes.

func CFLocaleCreateCanonicalLanguageIdentifierFromString(CFAllocator!, CFString!) -> CFLocaleIdentifier!

Returns a canonical language identifier by mapping an arbitrary locale identification string to the canonical identifier

func CFLocaleCreateCanonicalLocaleIdentifierFromString(CFAllocator!, CFString!) -> CFLocaleIdentifier!

Returns a canonical locale identifier by mapping an arbitrary locale identification string to the canonical identifier.

func CFLocaleCreateComponentsFromLocaleIdentifier(CFAllocator!, CFLocaleIdentifier!) -> CFDictionary!

Returns a dictionary containing the result from parsing a locale ID consisting of language, script, country or region, variant, and keyword/value pairs.

func CFLocaleCreateLocaleIdentifierFromComponents(CFAllocator!, CFDictionary!) -> CFLocaleIdentifier!

Returns a locale identifier consisting of language, script, country or region, variant, and keyword/value pairs derived from a dictionary containing the source information.

func CFLocaleCreateLocaleIdentifierFromWindowsLocaleCode(CFAllocator!, UInt32) -> CFLocaleIdentifier!

Returns a locale identifier from a Windows locale code.

func CFLocaleGetWindowsLocaleCodeFromLocaleIdentifier(CFLocaleIdentifier!) -> UInt32

Returns a Windows locale code from the locale identifier.

### Getting Line and Character Direction for a Language

func CFLocaleGetLanguageCharacterDirection(CFString!) -> CFLocaleLanguageDirection

Returns the character direction for the specified ISO language code.

func CFLocaleGetLanguageLineDirection(CFString!) -> CFLocaleLanguageDirection

Returns the line direction for the specified ISO language code.

### Getting the CFLocale Type ID

func CFLocaleGetTypeID() -> CFTypeID

Returns the type identifier for the CFLocale opaque type.

### Constants

enum CFLocaleLanguageDirection

These constants describe the text direction for a language. They are returned by the functions CFLocaleGetLanguageCharacterDirection(_:) and CFLocaleGetLanguageLineDirection(_:).

Locale Property Keys

Predefined locale keys used to get property values.

Locale Calendar Identifiers

Predefined locale keys used to get calendar values—values for `kCFLocaleCalendarIdentifier`.

Locale Change Notification

Identifier for notification sent if the current locale changes.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Internationalization and Localization Guide

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

