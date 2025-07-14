

- Foundation
- DateComponentsFormatter
- DateComponentsFormatter.UnitsStyle
-  DateComponentsFormatter.UnitsStyle.positional 

Case

# DateComponentsFormatter.UnitsStyle.positional

A style that uses the position of a unit of time to identify its value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case positional
```

## Discussion

This style is most commonly used for time values where the hour, minute, and second values are separated by colons. You can use the zero formatting behaviors (DateComponentsFormatter.ZeroFormattingBehavior) to further modify the formatting of this value.

For example, one hour and ten minutes is displayed in the U.S. English locale as “1:10:00”.

Note

This style may fall back to the behavior of DateComponentsFormatter.UnitsStyle.abbreviated when attempting to display large time quantities.

## See Also

### Styles

case spellOut

A style that spells out the units and quantities of time.

case full

A style that spells out the units of time, but not the quantities.

case short

A style that uses a shortened spelling for units.

case brief

A style that uses a shortened spelling for units of time that is shorter than DateComponentsFormatter.UnitsStyle.short.

case abbreviated

A style that uses the most abbreviated spelling for units of time.

case spellOut

A style that spells out the units and quantities of time.

case full

A style that spells out the units of time, but not the quantities.

case short

A style that uses a shortened spelling for units.

case brief

A style that uses a shortened spelling for units of time that is shorter than DateComponentsFormatter.UnitsStyle.short.

case abbreviated

A style that uses the most abbreviated spelling for units of time.

