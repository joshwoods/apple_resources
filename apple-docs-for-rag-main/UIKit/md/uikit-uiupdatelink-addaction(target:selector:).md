

- UIKit
- UIUpdateLink
-  addAction(target:selector:) 

Instance Method

# addAction(target:selector:)

Adds an action with the specified target and selector to the UI update link.

iOSiPadOStvOSvisionOS

``` source
@MainActor
func addAction(
    target: Any,
    selector: Selector
)
```

## Discussion

This method adds the action to the beforeCADisplayLinkDispatch phase. To specify a different phase, use addAction(to:target:selector:) instead.

## See Also

### Adding actions

func addAction(handler: (UIUpdateLink, UIUpdateInfo) -> Void)

Adds an action with the specified handler to the UI update link.

func addAction(to: UIUpdateActionPhase, handler: (UIUpdateLink, UIUpdateInfo) -> Void)

Adds an action with the specified handler to the UI update link for a particular UI update phase.

func addAction(to: UIUpdateActionPhase, target: Any, selector: Selector)

Adds an action with the specified target and selector to the UI update link for a particular UI update phase.

class UIUpdateActionPhase

An object that defines specific phases of the UI update process.

