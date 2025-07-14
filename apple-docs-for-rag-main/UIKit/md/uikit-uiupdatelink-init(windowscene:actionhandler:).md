

- UIKit
- UIUpdateLink
-  init(windowScene:actionHandler:) 

Initializer

# init(windowScene:actionHandler:)

Creates a UI update link for the specified window using the specified action handler.

iOSiPadOStvOSvisionOS

``` source
@MainActor
init(
    windowScene: UIWindowScene,
    actionHandler handler: @escaping (UIUpdateLink, UIUpdateInfo) -> Void
)
```

## Discussion

This initializer adds the action to the beforeCADisplayLinkDispatch phase. To specify a different phase, use addAction(to:handler:) or addAction(to:target:selector:) instead.

## See Also

### Creating a UI update link

init(view: UIView)

Creates a UI update link for the specified view.

init(view: UIView, actionHandler: (UIUpdateLink, UIUpdateInfo) -> Void)

Creates a UI update link for the specified view using the specified action handler.

init(view: UIView, actionTarget: Any, selector: Selector)

Creates a UI update link for the specified view using the specified target and action.

init(windowScene: UIWindowScene)

Creates a UI update link for the specified window.

init(windowScene: UIWindowScene, actionTarget: Any, selector: Selector)

Creates a UI update link for the specified window using the specified target and action.

