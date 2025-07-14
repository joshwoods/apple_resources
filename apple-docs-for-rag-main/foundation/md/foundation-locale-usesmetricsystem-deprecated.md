

- Foundation
- Locale
-  usesMetricSystem Deprecated

Instance Property

# usesMetricSystem

A Boolean that is true if the locale uses the metric system.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 8.0–16.0DeprecatedmacOS 10.10–13.0DeprecatedtvOS 9.0–16.0DeprecatedvisionOS 1.0+watchOS 2.0–9.0Deprecated

``` source
var usesMetricSystem: Bool { get }
```

Deprecated

Use \`measurementSystem\` instead

## Discussion

-seealso: MeasurementFormatter

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

var exemplarCharacterSet: CharacterSet?

The exemplar character set for the locale, or `nil` if has none.

var collationIdentifier: String?

The collation identifier for the locale, or `nil` if it has none.

var collatorIdentifier: String?

The collator identifier of the locale.

var decimalSeparator: String?

The decimal separator of the locale.

var groupingSeparator: String?

The grouping separator of the locale.

var currencyCode: String?

The currency code of the locale.

var currencySymbol: String?

The currency symbol of the locale.

