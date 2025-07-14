

- SwiftUI
- WKHostingController
-  updateBodyIfNeeded() 

Instance Method

# updateBodyIfNeeded()

Updates the interface controller’s set of views immediately, if updates are pending.

watchOS 6.0+

``` source
@MainActor @preconcurrency
func updateBodyIfNeeded()
```

## Discussion

Calling this method forces the hosting controller to update its current set of views, but only if there are pending changes. If there are no pending changes, this method does nothing.

To mark the interface controller as needing an update, call setNeedsBodyUpdate().

## See Also

### Updating the root view

func setNeedsBodyUpdate()

Invalidates the current SwiftUI views and triggers an update during the next cycle.

