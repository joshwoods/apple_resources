

- SwiftUI
- View
-  animation(\_:) 

Instance Method

# animation(\_:)

Applies the given animation to this view when this view changes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func animation(_ animation: Animation?) -> some View
```

Available when `Self` conforms to `Equatable`.

Show all declarations

## Parameters 

`animation`  

The animation to apply. If `animation` is `nil`, the view doesn’t animate.

## Return Value

A view that applies `animation` to this view whenever it changes.

## See Also

### Adding state-based animation to a view

func animation&lt;V>(Animation?, value: V) -> some View

Applies the given animation to this view when the specified value changes.

func animation&lt;V>(Animation?, body: (PlaceholderContentView&lt;Self>) -> V) -> some View

Applies the given animation to all animatable values within the `body` closure.

