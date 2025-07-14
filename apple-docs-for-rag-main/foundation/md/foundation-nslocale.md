

- Foundation
-  NSLocale 

Class

# NSLocale

Information about linguistic, cultural, and technological conventions for use in formatting data for presentation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSLocale
```

## Overview

In Swift, this object bridges to Locale; use NSLocale when you need reference semantics or other Foundation-specific behavior.

You typically use a locale to format and interpret information about and according to the user’s customs and preferences.

You can initialize any number of locale instances with init(localeIdentifier:) using one of the locale identifiers found in the availableLocaleIdentifiers array. However, you usually use a locale configured to match the preferences of the current user.

Use the current property to get the locale matching the current user’s preferences. If you need to be alerted when the user does make changes to region settings, register for the currentLocaleDidChangeNotification notification. Alternatively, you can use the autoupdatingCurrent property to get a locale that automatically updates with the user’s configuration settings:

- Swift
- Objective-C

```
let locale = NSLocale.autoupdatingCurrent
```

```
NSLocale* locale = [NSLocale autoupdatingCurrentLocale];
```

You can inspect a locale by reading its properties, as listed in Getting Information About a Locale. For properties containing a code or identifier, you can then obtain a string suitable for presentation to the user with the methods listed in Getting Display Information About a Locale. For example, you can report the user’s language as a string localized in that language using the autoupdating locale obtained in the previous example:

- Swift
- Objective-C

```
let code = locale.languageCode!
let language = locale.localizedString(forLanguageCode: code)!

print("\(language)")
// Prints "English" for locale en_US, "français" for fr_FR
```

```
NSString* code = locale.languageCode;
NSString* language = [locale localizedStringForLanguageCode:code];

NSLog(@"%@",language);
// Prints "English" for locale en_US, "français" for fr_FR
```

You frequently use a locale in conjunction with a formatter. For example, the DateFormatter class has a locale property that ensures dates are converted to strings that match the user’s expectations about date formatting. By default, this property indicates the user’s current locale, which is usually the behavior you want, but you can instead set it to another locale instance to obtain a different output. See Data Formatting Guide for more information about working with formatters.

NSLocale is *toll-free bridged* with its Core Foundation counterpart, CFLocale. See Toll-Free Bridging for more information on toll-free bridging.

Important

The Swift overlay to the Foundation framework provides the Locale structure, which bridges to the NSLocale class. For more information about value types, see Working with Cocoa Frameworks in Using Swift with Cocoa and Objective-C (Swift 4.1).

## Topics

### Initializing a Locale

init(localeIdentifier: String)

Initializes a locale using a given locale identifier.

init?(coder: NSCoder)

Returns a locale initialized from data in the given unarchiver.

### Getting the User’s Locale

class var autoupdatingCurrent: Locale

A locale which tracks the user’s current preferences.

class var current: Locale

A locale representing the user’s region settings at the time the property is read.

class let currentLocaleDidChangeNotification: NSNotification.Name

A notification that indicates that the user’s locale changed.

class var system: Locale

A locale representing the generic root values with little localization.

### Getting Known Identifiers and Codes

class var availableLocaleIdentifiers: [String]

The list of locale identifiers available on the system.

class var isoCountryCodes: [String]

The list of known country or region codes.

class var isoLanguageCodes: [String]

The list of known language codes.

class var isoCurrencyCodes: [String]

The list of known currency codes.

class var commonISOCurrencyCodes: [String]

A list of commonly encountered currency codes.

### Converting Between Identifiers

class func canonicalLocaleIdentifier(from: String) -> String

Returns the canonical identifier for a given locale identification string.

class func components(fromLocaleIdentifier: String) -> [String : String]

Returns a dictionary that is the result of parsing a locale ID.

class func localeIdentifier(fromComponents: [String : String]) -> String

Returns a locale identifier from the components specified in a given dictionary.

class func canonicalLanguageIdentifier(from: String) -> String

Returns a canonical language identifier by mapping an arbitrary locale identification string to the canonical identifier.

class func localeIdentifier(fromWindowsLocaleCode: UInt32) -> String?

Returns a locale identifier from a Windows locale code.

class func windowsLocaleCode(fromLocaleIdentifier: String) -> UInt32

Returns a Window locale code from the locale identifier.

### Getting Information About a Locale

var localeIdentifier: String

The identifier for the locale.

var countryCode: String?

The country or region code for the locale.

var languageCode: String

The language code for the locale.

var scriptCode: String?

The script code for the locale.

var variantCode: String?

The variant code for the locale.

var exemplarCharacterSet: CharacterSet

The exemplar character set for the locale.

var collationIdentifier: String?

The collation identifier for the locale.

var collatorIdentifier: String

The collator identifier for the locale.

var usesMetricSystem: Bool

A Boolean value that indicates whether the locale uses the metric system.

var decimalSeparator: String

The decimal separator for the locale.

var groupingSeparator: String

The grouping separator for the locale.

var currencyCode: String?

The currency code for the locale.

var currencySymbol: String

The currency symbol for the locale.

var calendarIdentifier: String

The calendar identifier for the locale.

var quotationBeginDelimiter: String

The begin quotation symbol for the locale.

var quotationEndDelimiter: String

The end quotation symbol for the locale.

var alternateQuotationBeginDelimiter: String

The alternate begin quotation symbol for the locale.

var alternateQuotationEndDelimiter: String

The alternate end quotation symbol for the locale.

### Getting Display Information About a Locale

func localizedString(forLocaleIdentifier: String) -> String

Returns the localized string for the specified locale identifier.

func localizedString(forCountryCode: String) -> String?

Returns the localized string for a country or region code.

func localizedString(forLanguageCode: String) -> String?

Returns the localized string for the specified language code.

func localizedString(forScriptCode: String) -> String?

Returns the localized string for the specified script code.

func localizedString(forVariantCode: String) -> String?

Returns the localized string for the specified variant code.

func localizedString(forCollationIdentifier: String) -> String?

Returns the localized string for the specified collation identifier.

func localizedString(forCollatorIdentifier: String) -> String?

Returns the localized string for the specified collator identifier.

func localizedString(forCurrencyCode: String) -> String?

Returns the localized string for the specified currency code.

func localizedString(forCalendarIdentifier: String) -> String?

Returns the localized string for the specified calendar identifier.

Locale Calendar Identifiers

The types of calendars.

### Accessing Locale Information by Key

func object(forKey: NSLocale.Key) -> Any?

Returns the value of the component corresponding to the specified key.

func displayName(forKey: NSLocale.Key, value: Any) -> String?

Returns the display name for the given locale component value.

struct Key

The keys used to access components of a locale.

### Getting the User’s Preferred Languages

class var preferredLanguages: [String]

An ordered list of the user’s preferred languages.

### Getting Line and Character Direction for a Language

class func characterDirection(forLanguage: String) -> NSLocale.LanguageDirection

Returns the direction of the sequence of characters in a line for the specified ISO language code.

class func lineDirection(forLanguage: String) -> NSLocale.LanguageDirection

Returns the direction of the sequence of lines for the specified ISO language code.

enum LanguageDirection

The directions that a language may take across a page of text.

### Instance Properties

var languageIdentifier: String

var regionCode: String?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Related Documentation

Internationalization and Localization Guide

Data Formatting Guide

