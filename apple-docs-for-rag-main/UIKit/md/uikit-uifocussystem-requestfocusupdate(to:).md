

- UIKit
- UIFocusSystem
-  requestFocusUpdate(to:) 

Instance Method

# requestFocusUpdate(to:)

Submits a request to update the focus state of the specified object.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
@MainActor
func requestFocusUpdate(to environment: any UIFocusEnvironment)
```

## Parameters 

`environment`  

The view, view controller, window, or other object that you want to update. You can specify any object that adopts the UIFocusEnvironment protocol.

## Discussion

Use this method to ask the focus engine to update the focus-related information for the specified object. If the update request is accepted, the focus engine updates the object’s focus-related information during the next run loop cycle. If the specified object does not contain a focused item, calling this method has no effect.

## See Also

### Managing focus updates

func updateFocusIfNeeded()

Forces the system to act on a pending focus update for the current environment.

