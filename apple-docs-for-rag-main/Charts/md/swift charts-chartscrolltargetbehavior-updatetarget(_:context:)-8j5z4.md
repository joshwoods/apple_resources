

- Swift Charts
- ChartScrollTargetBehavior
-  updateTarget(\_:context:) 

Instance Method

# updateTarget(\_:context:)

Updates the proposed target that a scrollable view should scroll to.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func updateTarget(
    _ target: inout ScrollTarget,
    context: ScrollTargetBehaviorContext
)
```

## Discussion

The system calls this method in two main cases:

- When a scroll gesture ends, it calculates where it would naturally scroll to using its deceleration rate. The system provides this calculated value as the target of this method.

- When a scrollable view’s size changes, it calculates where it should be scrolled given the new size and provides this calculates value as the target of this method.

You can implement this method to override the calculated target which will have the scrollable view scroll to a different position than it would otherwise.

