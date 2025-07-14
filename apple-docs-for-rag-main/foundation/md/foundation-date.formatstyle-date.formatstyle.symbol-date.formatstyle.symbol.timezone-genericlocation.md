

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.TimeZone
-  genericLocation 

Type Property

# genericLocation

The generic location representation of a timezone.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var genericLocation: Date.FormatStyle.Symbol.TimeZone { get }
```

## Discussion

If the generic location is unavailable, the system provides the value of localizedGMT(_:) with a `long` width. For example, `Los Angeles Time`.

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

static var exemplarLocation: Date.FormatStyle.Symbol.TimeZone

The exemplar city for a timezone.

