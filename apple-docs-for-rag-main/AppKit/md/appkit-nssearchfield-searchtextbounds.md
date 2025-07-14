

- AppKit
- NSSearchField
-  searchTextBounds 

Instance Property

# searchTextBounds

The rectangle for the search text within the bounds of the search field.

macOS 11.0+

``` source
@MainActor
var searchTextBounds: NSRect { get }
```

## Discussion

Subclasses can override `searchTextBounds` for custom layout purposes.

## See Also

### Getting Search Field Metrics

var cancelButtonBounds: NSRect

The rectangle for the cancel button within the bounds of the search field.

var searchButtonBounds: NSRect

The rectangle for the search button within the bounds of the search field.

