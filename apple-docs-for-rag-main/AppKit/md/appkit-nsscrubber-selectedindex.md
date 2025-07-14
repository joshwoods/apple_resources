

- AppKit
- NSScrubber
-  selectedIndex 

Instance Property

# selectedIndex

The index of the selected item in the scrubber.

macOS 10.12.2+

``` source
@MainActor
var selectedIndex: Int { get set }
```

## Discussion

If no item is selected, the value of this property is `-1`. If you set this property through the scrubber’s animator proxy, the selection change animates.

To use a scrubber’s animator proxy when changing the selected item, employ the NSAnimatablePropertyContainer protocol, using code like this: `scrubber.animator.selectedIndex = 123`

## See Also

### Getting the state of the scrubber

var numberOfItems: Int

The number of items represented by the scrubber.

var highlightedIndex: Int

The index of the highlighted item in the scrubber.

