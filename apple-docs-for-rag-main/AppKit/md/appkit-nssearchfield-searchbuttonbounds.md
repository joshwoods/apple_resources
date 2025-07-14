

- AppKit
- NSSearchField
-  searchButtonBounds 

Instance Property

# searchButtonBounds

The rectangle for the search button within the bounds of the search field.

macOS 11.0+

``` source
@MainActor
var searchButtonBounds: NSRect { get }
```

## Discussion

Subclasses can override `searchButtonBounds` for custom layout purposes.

## See Also

### Getting Search Field Metrics

var cancelButtonBounds: NSRect

The rectangle for the cancel button within the bounds of the search field.

var searchTextBounds: NSRect

The rectangle for the search text within the bounds of the search field.

