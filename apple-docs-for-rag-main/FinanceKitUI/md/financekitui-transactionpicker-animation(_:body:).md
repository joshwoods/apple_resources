

- FinanceKitUI
- TransactionPicker
-  animation(\_:body:) 

Instance Method

# animation(\_:body:)

Applies the given animation to all animatable values within the `body` closure.

FinanceKitUISwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
func animation(
    _ animation: Animation?,
    @ViewBuilder body: (PlaceholderContentView) -> V
) -> some View where V : View
```

## Discussion

Any modifiers applied to the content of `body` will be applied to this view, and the `animation` will only be used on the modifiers defined in the `body`.

The following code animates the opacity changing with an easeInOut animation, while the contents of MyView are animated with the implicit transaction’s animation:

```
MyView(isActive: isActive)
    .animation(.easeInOut) { content in
        content.opacity(isActive ? 1.0 : 0.0)
    }
```

