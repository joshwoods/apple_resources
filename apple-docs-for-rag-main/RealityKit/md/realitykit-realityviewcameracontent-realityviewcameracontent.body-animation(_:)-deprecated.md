

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  animation(\_:) Deprecated

Instance Method

# animation(\_:)

Applies the given animation to all animatable values within this view.

RealityKitSwiftUIiOS 13.0–15.0DeprecatediPadOS 13.0–15.0DeprecatedMac CatalystmacOS 10.15–12.0DeprecatedtvOS 13.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 6.0–8.0Deprecated

``` source
nonisolated
func animation(_ animation: Animation?) -> some View
```

Deprecated

Use withAnimation or animation(\_:value:) instead.

## Parameters 

`animation`  

The animation to apply to animatable values within this view.

## Return Value

A view that wraps this view and applies `animation` to all animatable values used within the view.

## Discussion

Use this modifier on leaf views rather than container views. The animation applies to all child views within this view; calling `animation(_:)` on a container view can lead to unbounded scope.

