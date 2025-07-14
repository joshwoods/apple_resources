

- App Intents
- SiriTipView
-  scaleEffect(\_:anchor:) 

Instance Method

# scaleEffect(\_:anchor:)

Scales this view uniformly by the specified factor.

AppIntentsSwiftUIvisionOS 1.0+

``` source
nonisolated
func scaleEffect(
    _ s: CGFloat,
    anchor: UnitPoint3D = .center
) -> some View
```

## Parameters 

`s`  

The scale factor for this view.

`anchor`  

The anchor point about which to scale the view. Defaults to center.

## Return Value

A view that scales this view by `s` in all dimensions.

## Discussion

The original dimensions of the view are considered to be unchanged by scaling the contents. To change the dimensions of the view, use a modifier like `frame()` instead.

