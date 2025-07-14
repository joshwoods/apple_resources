

- UIKit
- UIFocusGuide
-  preferredFocusEnvironments 

Instance Property

# preferredFocusEnvironments

An array of focus environments to which the guide directs focus, ordered by priority.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var preferredFocusEnvironments: [any UIFocusEnvironment]! { get set }
```

## Mentioned in 

About focus interactions for Apple TV

Creating custom navigation interactions

## Discussion

Setting this property to a nonempty array marks this guide’s layoutFrame as focusable. If empty, this guide is effectively disabled.

If focused, the guide attempts to redirect focus to each environment in the array, in order, stopping when a focusable item in an environment has been found.

## See Also

### Enabling focus

var isEnabled: Bool

A Boolean value that indicates whether the guide is focusable.

var preferredFocusedView: UIView?

The view that the focus will be redirected to if this guide is focused.

Deprecated

