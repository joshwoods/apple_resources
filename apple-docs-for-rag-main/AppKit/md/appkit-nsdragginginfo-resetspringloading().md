

- AppKit
- NSDraggingInfo
-  resetSpringLoading() 

Instance Method

# resetSpringLoading()

Resets a spring-loading operation to its initial state.

macOS 10.11+

``` source
@MainActor
func resetSpringLoading()
```

**Required**

## Discussion

Call this method when a drag operation moves from one spring-loaded region into another within the same destination and the spring-loading options haven’t changed.

For example, consider an NSSegmentedControl object. It’s a single spring-loading destination. However, each segment within the control can be individually spring-loaded. Each time the drag enters a new segment within the control, the spring-loading destination and options don’t change. NSSegmentedControl calls the resetSpringLoading() method to reset the spring-loading operation for the newly entered segment.

When this method is called, the spring-loading operation is reset. Hover time required to activate spring-loading is reset and begins again. If a force click is currently active, the user must reduce pressure enough to disengage the force click. Then, the user must force click again to activate the newly entered spring-loaded region.

## See Also

### Implementing spring-loading support

var springLoadingHighlight: NSSpringLoadingHighlight

A highlighting style for your app’s user interface to display during a spring-loading operation.

**Required**

