

- Foundation
- Date
- 
  - Date
- Date.FormatStyle
- Date.FormatStyle.Symbol
- Date.FormatStyle.Symbol.TimeZone
-  identifier(\_:) 

Type Method

# identifier(\_:)

Returns the timezone identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func identifier(_ width: Date.FormatStyle.Symbol.TimeZone.Width) -> Date.FormatStyle.Symbol.TimeZone
```

## Parameters 

`width`  

Specifies the width of the string result.

## Return Value

A timezone format style appropriate for the locale and specified width.

## Discussion

For example, `uslax` (Date.FormatStyle.Symbol.TimeZone.Width.short) or `America/Los_Angeles` (Date.FormatStyle.Symbol.TimeZone.Width.long).

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

static var exemplarLocation: Date.FormatStyle.Symbol.TimeZone

The exemplar city for a timezone.

static var genericLocation: Date.FormatStyle.Symbol.TimeZone

The generic location representation of a timezone.

