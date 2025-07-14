

- Foundation
- Date
- Date.RelativeFormatStyle
- Date.RelativeFormatStyle.UnitsStyle
-  abbreviated 

Type Property

# abbreviated

A style that uses abbreviated units, such as “2 mo. ago”.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var abbreviated: Date.RelativeFormatStyle.UnitsStyle { get }
```

## Discussion

This style may give different results in languages other than English.

## See Also

### Modifying a Relative Date Format Units Style

static var narrow: Date.RelativeFormatStyle.UnitsStyle

A style that uses the shortest units, such as “2 mo. ago”.

static var spellOut: Date.RelativeFormatStyle.UnitsStyle

A style that spells out units, such as “two months ago”.

static var wide: Date.RelativeFormatStyle.UnitsStyle

A style that uses full representation of units, such as “2 months ago”.

