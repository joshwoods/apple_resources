

- Foundation
- Locale
-  exemplarCharacterSet 

Instance Property

# exemplarCharacterSet

The exemplar character set for the locale, or `nil` if has none.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var exemplarCharacterSet: CharacterSet? { get }
```

## See Also

### Getting information about a locale

var identifier: String

The identifier of the locale.

func identifier(Locale.IdentifierType) -> String

Returns the locale identifier, in the specified standard format.

enum IdentifierType

A type that indicates the standard that defines a locale’s identifier.

var calendar: Calendar

The calendar for the locale, or the Gregorian calendar as a fallback.

var regionCode: String?

The region code of the locale, or `nil` if it has none.

var languageCode: String?

The language code of the locale, or `nil` if has none.

var scriptCode: String?

The script code of the locale, or `nil` if has none.

var variantCode: String?

The variant code for the locale, or `nil` if it has none.

var collationIdentifier: String?

The collation identifier for the locale, or `nil` if it has none.

var collatorIdentifier: String?

The collator identifier of the locale.

var usesMetricSystem: Bool

A Boolean that is true if the locale uses the metric system.

Deprecated

var decimalSeparator: String?

The decimal separator of the locale.

var groupingSeparator: String?

The grouping separator of the locale.

var currencyCode: String?

The currency code of the locale.

var currencySymbol: String?

The currency symbol of the locale.

