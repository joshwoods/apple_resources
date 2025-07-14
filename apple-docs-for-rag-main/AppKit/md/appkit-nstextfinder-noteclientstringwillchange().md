

- AppKit
- NSTextFinder
-  noteClientStringWillChange() 

Instance Method

# noteClientStringWillChange()

Invoke this method when the searched content will change.

macOS 10.7+

``` source
func noteClientStringWillChange()
```

## Discussion

When incremental search is enabled, this method must be called when it is known that the client’s string will be modified. This method must be called before the client string modification takes place.

## See Also

### Related Documentation

var client: (any NSTextFinderClient)?

The object that provides the target search string, find bar location, and feedback methods.

