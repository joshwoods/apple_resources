

- UIKit
- UIFocusEnvironment
-  didUpdateFocus(in:with:) 

Instance Method

# didUpdateFocus(in:with:)

Called immediately after the system updates the focus to a new view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func didUpdateFocus(
    in context: UIFocusUpdateContext,
    with coordinator: UIFocusAnimationCoordinator
)
```

**Required**

## Parameters 

`context`  

An instance of UIFocusUpdateContext containing metadata of the focus related update.

`coordinator`  

An instance of UIFocusAnimationCoordinator used for coordinating focus-related animations.

## Discussion

After the focus is updated to a new view, the focus engine calls this method on all focus environments that contain either the previously focused view, the next focused view, or both, in ascending order. You should override this method to update your app’s state in response to changes in focus. Use the provided animation coordinator to animate changes in visual appearance related to the update. For more information on animation coordinators, see UIFocusAnimationCoordinator.

