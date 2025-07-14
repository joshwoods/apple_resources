

- AppKit
- NSSearchField
-  cancelButtonBounds 

Instance Property

# cancelButtonBounds

The rectangle for the cancel button within the bounds of the search field.

macOS 11.0+

``` source
@MainActor
var cancelButtonBounds: NSRect { get }
```

## Discussion

Subclasses can override `cancelButtonBounds` for custom layout purposes.

## See Also

### Getting Search Field Metrics

var searchButtonBounds: NSRect

The rectangle for the search button within the bounds of the search field.

var searchTextBounds: NSRect

The rectangle for the search text within the bounds of the search field.

