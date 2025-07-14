

- UIKit
- UIUpdateLink
-  init(windowScene:) 

Initializer

# init(windowScene:)

Creates a UI update link for the specified window.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
init(windowScene: UIWindowScene)
```

## See Also

### Creating a UI update link

init(view: UIView)

Creates a UI update link for the specified view.

init(view: UIView, actionHandler: (UIUpdateLink, UIUpdateInfo) -> Void)

Creates a UI update link for the specified view using the specified action handler.

init(view: UIView, actionTarget: Any, selector: Selector)

Creates a UI update link for the specified view using the specified target and action.

init(windowScene: UIWindowScene, actionHandler: (UIUpdateLink, UIUpdateInfo) -> Void)

Creates a UI update link for the specified window using the specified action handler.

init(windowScene: UIWindowScene, actionTarget: Any, selector: Selector)

Creates a UI update link for the specified window using the specified target and action.

