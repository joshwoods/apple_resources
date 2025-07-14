

- UIKit
- UIUpdateLink
-  addAction(handler:) 

Instance Method

# addAction(handler:)

Adds an action with the specified handler to the UI update link.

iOSiPadOStvOSvisionOS

``` source
@MainActor
func addAction(handler: @escaping (UIUpdateLink, UIUpdateInfo) -> Void)
```

## Discussion

This method adds the action to the beforeCADisplayLinkDispatch phase. To specify a different phase, use addAction(to:handler:) instead.

## See Also

### Adding actions

func addAction(to: UIUpdateActionPhase, handler: (UIUpdateLink, UIUpdateInfo) -> Void)

Adds an action with the specified handler to the UI update link for a particular UI update phase.

func addAction(target: Any, selector: Selector)

Adds an action with the specified target and selector to the UI update link.

func addAction(to: UIUpdateActionPhase, target: Any, selector: Selector)

Adds an action with the specified target and selector to the UI update link for a particular UI update phase.

class UIUpdateActionPhase

An object that defines specific phases of the UI update process.

