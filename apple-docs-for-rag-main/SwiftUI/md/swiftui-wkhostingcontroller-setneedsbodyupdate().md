

- SwiftUI
- WKHostingController
-  setNeedsBodyUpdate() 

Instance Method

# setNeedsBodyUpdate()

Invalidates the current SwiftUI views and triggers an update during the next cycle.

watchOS 6.0+

``` source
@MainActor @preconcurrency
func setNeedsBodyUpdate()
```

## Discussion

Call this method to mark the views of the hosting controller as needing an update. During the next update cycle, the hosting controller fetches an updated set of views from its body property.

## See Also

### Updating the root view

func updateBodyIfNeeded()

Updates the interface controller’s set of views immediately, if updates are pending.

