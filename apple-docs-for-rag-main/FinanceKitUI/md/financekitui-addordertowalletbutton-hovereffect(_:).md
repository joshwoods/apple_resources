

- FinanceKitUI
- AddOrderToWalletButton
-  hoverEffect(\_:) 

Instance Method

# hoverEffect(\_:)

Applies a hover effect to this view.

FinanceKitUISwiftUIiOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+tvOS 16.0+visionOS 1.0+

``` source
nonisolated
func hoverEffect(_ effect: HoverEffect = .automatic) -> some View
```

## Parameters 

`effect`  

The effect to apply to this view.

`isEnabled`  

Whether the effect is enabled or not.

## Return Value

A new view that applies a hover effect to `self`.

## Discussion

By default, `HoverEffect/automatic` is used. You can control the behavior of the automatic effect with the `View/defaultHoverEffect(_:)` modifier.

