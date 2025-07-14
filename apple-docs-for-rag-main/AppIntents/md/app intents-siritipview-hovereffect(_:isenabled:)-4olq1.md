

- App Intents
- SiriTipView
-  hoverEffect(\_:isEnabled:) 

Instance Method

# hoverEffect(\_:isEnabled:)

Applies a hover effect to this view.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+tvOS 17.0+visionOS 1.0+

``` source
nonisolated
func hoverEffect(
    _ effect: HoverEffect = .automatic,
    isEnabled: Bool = true
) -> some View
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

