

- Foundation
- ListFormatStyle
-  listType 

Instance Property

# listType

The type of the list.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var listType: ListFormatStyle.ListType
```

## Discussion

The list type determines the semantics used in the return string.

For example, for en_US:

```
["One", "Two", "Three"].formatted(.list(type: .and))
// “One, Two, and Three”

["One", "Two", "Three"].formatted(.list(type: .or))
// “One, Two, or Three” 
```

The default value is ListFormatStyle.ListType.and.

## See Also

### Modifying a list format style

var width: ListFormatStyle&lt;Style, Base>.Width

The size of the list.

enum Width

The type representing the width of a list.

enum ListType

A type that describes whether the returned list contains cumulative or alternative elements.

var locale: Locale

The locale to use when formatting items in the list.

