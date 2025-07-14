

- UIKit
- UIFocusGuide
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the guide is focusable.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

If the value of this property is true (the default), then the guide may be focusable. Some conditions, defined by the system, may prevent the guide from being focusable even if it’s enabled, such as when the guide’s frame overlaps with the currently focused view. However, if this property is set to false, then the guide isn’t focusable.

## See Also

### Enabling focus

var preferredFocusEnvironments: [any UIFocusEnvironment]!

An array of focus environments to which the guide directs focus, ordered by priority.

var preferredFocusedView: UIView?

The view that the focus will be redirected to if this guide is focused.

Deprecated

