

- Foundation
- ListFormatter
-  itemFormatter 

Instance Property

# itemFormatter

An object that formats each item in the list.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@NSCopying
var itemFormatter: Formatter? { get set }
```

## Discussion

If this property isn’t set, the list formatter falls back to the item’s description(withLocale:) or localizedDescription methods if implemented. If those methods aren’t implemented, the formatter uses description instead.

## See Also

### Configuring Formatter Options

var locale: Locale!

The locale to use when formatting items in the list.

