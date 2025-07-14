

- UIKit
- UIFocusEnvironment
-  preferredFocusedView Deprecated

Instance Property

# preferredFocusedView

Specifies the view that should be focused if this environment is focused.

iOS 9.0–10.0DeprecatediPadOS 9.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–10.0Deprecated

``` source
@MainActor
weak optional var preferredFocusedView: UIView? { get }
```

Deprecated

Use preferredFocusEnvironments instead.

## Discussion

Since UIView conforms to UIFocusEnvironment, any view returned from this property also has a preferred focused view. This creates a linked-list of views called the *preferred focus chain*. When focus updates to a new view, the focus engine will actually update focus to the deepest, focusable view in that new view’s preferred focus chain. Similarly, when setting initial focus, such as at application launch, the initial focused view is found by following the preferred focus chain from the root window.

By default, UIView returns itself and UIViewController returns its root view. Returning `self` in a focusable view indicates that view should be focused. Returning `self` in an unfocusable view causes the focus engine to pick a default preferred focused view, by finding the closest focusable subview to the top-leading corner of the screen. Returning `nil` indicates that there is no preferred focused view.

## See Also

### Controlling user-generated focus movements

var preferredFocusEnvironments: [any UIFocusEnvironment]

An array of focus environments, ordered by priority, to which this environment prefers focus to be directed during a focus update.

**Required**

