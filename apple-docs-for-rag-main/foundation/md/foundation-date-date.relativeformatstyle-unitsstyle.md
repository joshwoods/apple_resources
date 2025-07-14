

- Foundation
- Date
- Date.RelativeFormatStyle
-  unitsStyle 

Instance Property

# unitsStyle

The style to use when formatting the quantity or the name of the unit, such as “1 day ago” or “one day ago”.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var unitsStyle: Date.RelativeFormatStyle.UnitsStyle
```

## Discussion

Express relative date format units in either ```` wide```,`  ````narrow``` ,` ``abbreviated ```,\` or `spellOut` styles. For example:

```
if let past = Calendar.current.date(byAdding: .day, value: -14, to: Date()) {
    past.formatted(.relative(presentation: .named, unitsStyle: .wide)) // "2 weeks ago"
    past.formatted(.relative(presentation: .named, unitsStyle: .narrow)) // "2 wk. ago"
    past.formatted(.relative(presentation: .named, unitsStyle: .abbreviated)) // "2 wk. ago"
    past.formatted(.relative(presentation: .named, unitsStyle: .spellOut)) // "two weeks ago"
}
```

## See Also

### Modifying a Relative Date Format Style

var presentation: Date.RelativeFormatStyle.Presentation

Specifies the style to use when describing a relative date, such as “1 day ago” or “yesterday”.

var calendar: Calendar

The calendar to use when formatting relative dates.

var capitalizationContext: FormatStyleCapitalizationContext

The capitalization context to use when formatting the relative dates.

var locale: Locale

The locale to use when formatting the relative date.

