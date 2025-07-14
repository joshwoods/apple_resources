

- SwiftUI
- View
-  animation(\_:value:) 

Instance Method

# animation(\_:value:)

Applies the given animation to this view when the specified value changes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func animation(
    _ animation: Animation?,
    value: V
) -> some View where V : Equatable
```

## Parameters 

`animation`  

The animation to apply. If `animation` is `nil`, the view doesn’t animate.

`value`  

A value to monitor for changes.

## Return Value

A view that applies `animation` to this view whenever `value` changes.

## Mentioned in 

Managing user interface state

## See Also

### Adding state-based animation to a view

func animation(_:)

Applies the given animation to this view when this view changes.

func animation&lt;V>(Animation?, body: (PlaceholderContentView&lt;Self>) -> V) -> some View

Applies the given animation to all animatable values within the `body` closure.

