

- AppKit
- NSScrubber
-  highlightedIndex 

Instance Property

# highlightedIndex

The index of the highlighted item in the scrubber.

macOS 10.12.2+

``` source
@MainActor
var highlightedIndex: Int { get }
```

## Discussion

If no item is highlighted, the value of this property is `-1`.

## See Also

### Getting the state of the scrubber

var numberOfItems: Int

The number of items represented by the scrubber.

var selectedIndex: Int

The index of the selected item in the scrubber.

