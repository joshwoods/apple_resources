

- UIKit
- UIUpdateLink
-  init(view:actionTarget:selector:) 

Initializer

# init(view:actionTarget:selector:)

Creates a UI update link for the specified view using the specified target and action.

iOSiPadOStvOSvisionOS

``` source
@MainActor
init(
    view: UIView,
    actionTarget target: Any,
    selector: Selector
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

init(windowScene: UIWindowScene)

Creates a UI update link for the specified window.

init(windowScene: UIWindowScene, actionHandler: (UIUpdateLink, UIUpdateInfo) -> Void)

Creates a UI update link for the specified window using the specified action handler.

init(windowScene: UIWindowScene, actionTarget: Any, selector: Selector)

Creates a UI update link for the specified window using the specified target and action.

