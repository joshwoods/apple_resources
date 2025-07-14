

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.TimeZone
-  exemplarLocation 

Type Property

# exemplarLocation

The exemplar city for a timezone.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var exemplarLocation: Date.FormatStyle.Symbol.TimeZone { get }
```

## Discussion

If the exemplar city is unavailable, the system provides the localized exemplar city name for the special zone or `unknown`. For example, `Los Angeles`.

## See Also

### Modifying a Time Zone

static func specificName(Date.FormatStyle.Symbol.TimeZone.Width) -> Date.FormatStyle.Symbol.TimeZone

Returns the specific, non-location representation of a timezone.

static func genericName(Date.FormatStyle.Symbol.TimeZone.Width) -> Date.FormatStyle.Symbol.TimeZone

Returns the generic, non-location representation of a timezone.

static func iso8601(Date.FormatStyle.Symbol.TimeZone.Width) -> Date.FormatStyle.Symbol.TimeZone

Creates the ISO 8601 representation of the timezone with hours, minutes, and optional seconds.

static func localizedGMT(Date.FormatStyle.Symbol.TimeZone.Width) -> Date.FormatStyle.Symbol.TimeZone

Returns the localized GMT format representation of a timezone.

static func identifier(Date.FormatStyle.Symbol.TimeZone.Width) -> Date.FormatStyle.Symbol.TimeZone

Returns the timezone identifier.

static var genericLocation: Date.FormatStyle.Symbol.TimeZone

The generic location representation of a timezone.

