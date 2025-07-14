

- UIKit
- UIFocusGuide
-  preferredFocusedView Deprecated

Instance Property

# preferredFocusedView

The view that the focus will be redirected to if this guide is focused.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–10.0Deprecated

``` source
@MainActor
weak var preferredFocusedView: UIView? { get set }
```

Deprecated

Use preferredFocusEnvironments instead.

## Discussion

If the guide is focused, it indirects the focus to this view. This view, or at least one view along its preferredFocusedView chain, must be focusable in order for the guide to be focusable. Otherwise, it’s effectively disabled.

## See Also

### Enabling focus

var isEnabled: Bool

A Boolean value that indicates whether the guide is focusable.

var preferredFocusEnvironments: [any UIFocusEnvironment]!

An array of focus environments to which the guide directs focus, ordered by priority.

