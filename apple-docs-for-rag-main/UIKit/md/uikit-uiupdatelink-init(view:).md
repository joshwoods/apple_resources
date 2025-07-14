

- UIKit
- UIUpdateLink
-  init(view:) 

Initializer

# init(view:)

Creates a UI update link for the specified view.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
init(view: UIView)
```

## See Also

### Creating a UI update link

init(view: UIView, actionHandler: (UIUpdateLink, UIUpdateInfo) -> Void)

Creates a UI update link for the specified view using the specified action handler.

init(view: UIView, actionTarget: Any, selector: Selector)

Creates a UI update link for the specified view using the specified target and action.

init(windowScene: UIWindowScene)

Creates a UI update link for the specified window.

init(windowScene: UIWindowScene, actionHandler: (UIUpdateLink, UIUpdateInfo) -> Void)

Creates a UI update link for the specified window using the specified action handler.

init(windowScene: UIWindowScene, actionTarget: Any, selector: Selector)

Creates a UI update link for the specified window using the specified target and action.

