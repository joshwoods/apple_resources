

- Foundation
- ListFormatStyle
-  width 

Instance Property

# width

The size of the list.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var width: ListFormatStyle.Width
```

## Discussion

The `width` property controls the size of the list. The locale determines the formatting and abbreviation of the string for the given `width`.

For example, for English:

```
["One", "Two", "Three"].formatted(.list(type: .and, width: .standard))
// “One, Two, and Three”

["One", "Two", "Three"].formatted(.list(type: .and, width: .short))
// “One, Two, & Three” 

["One", "Two", "Three"].formatted(.list(type: .and, width: .narrow))
// “One, Two, Three” 
```

The default value is ListFormatStyle.Width.standard.

## See Also

### Modifying a list format style

enum Width

The type representing the width of a list.

var listType: ListFormatStyle&lt;Style, Base>.ListType

The type of the list.

enum ListType

A type that describes whether the returned list contains cumulative or alternative elements.

var locale: Locale

The locale to use when formatting items in the list.

