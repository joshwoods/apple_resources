

- UIKit
- UIFocusEnvironment
-  setNeedsFocusUpdate() 

Instance Method

# setNeedsFocusUpdate()

Submits a request to the focus engine for a focus update in this environment.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func setNeedsFocusUpdate()
```

**Required**

## Discussion

If this environment does not currently contain the focused view, calling this method has no effect. Otherwise, and if the focus update is accepted by the focus engine, focus is reset to the preferred focused view on the run loop cycle. If a parent of this environment is also requesting focus, the parent’s request takes priority.

## See Also

### Requesting focus update

func updateFocusIfNeeded()

Tells the focus engine to force a focus update immediately.

**Required**

