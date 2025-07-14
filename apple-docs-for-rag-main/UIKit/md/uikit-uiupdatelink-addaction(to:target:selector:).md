

- UIKit
- UIUpdateLink
-  addAction(to:target:selector:) 

Instance Method

# addAction(to:target:selector:)

Adds an action with the specified target and selector to the UI update link for a particular UI update phase.

iOS 18.0+iPadOS 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
func addAction(
    to phase: UIUpdateActionPhase,
    target: Any,
    selector: Selector
)
```

## See Also

### Adding actions

func addAction(handler: (UIUpdateLink, UIUpdateInfo) -> Void)

Adds an action with the specified handler to the UI update link.

func addAction(to: UIUpdateActionPhase, handler: (UIUpdateLink, UIUpdateInfo) -> Void)

Adds an action with the specified handler to the UI update link for a particular UI update phase.

func addAction(target: Any, selector: Selector)

Adds an action with the specified target and selector to the UI update link.

class UIUpdateActionPhase

An object that defines specific phases of the UI update process.

