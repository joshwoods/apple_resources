

- MusicKit
- ArtworkImage
-  hoverEffect(\_:isEnabled:) 

Instance Method

# hoverEffect(\_:isEnabled:)

Applies a hover effect to this view, while providing a way to conditionally enable or disable it.

MusicKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
nonisolated
func hoverEffect(
    _ effect: some CustomHoverEffect = .automatic,
    isEnabled: Bool = true
) -> some View
```

## Parameters 

`effect`  

The hover effect to apply to this view.

`isEnabled`  

Whether the hover effect is enabled or not.

## Return Value

A view with the hover effect applied.

## Discussion

By default, `CustomHoverEffect/automatic` is used. You can control the behavior of the automatic effect with the `View/defaultHoverEffect(_:)` modifier.

