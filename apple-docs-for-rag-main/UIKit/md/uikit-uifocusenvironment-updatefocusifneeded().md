

- UIKit
- UIFocusEnvironment
-  updateFocusIfNeeded() 

Instance Method

# updateFocusIfNeeded()

Tells the focus engine to force a focus update immediately.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func updateFocusIfNeeded()
```

**Required**

## Discussion

If any focus environment is currently pending an update (after calling setNeedsFocusUpdate()), then calling this method forces the focus engine to immediately update focus. Unlike setNeedsFocusUpdate(), it does not matter if this environment currently contains focus, or if this environment is the one pending an update.

## See Also

### Requesting focus update

func setNeedsFocusUpdate()

Submits a request to the focus engine for a focus update in this environment.

**Required**

