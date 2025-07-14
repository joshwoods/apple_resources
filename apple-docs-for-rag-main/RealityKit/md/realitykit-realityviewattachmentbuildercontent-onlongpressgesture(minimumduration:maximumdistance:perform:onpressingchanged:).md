

- RealityKit
- RealityViewAttachmentBuilderContent
-  onLongPressGesture(minimumDuration:maximumDistance:perform:onPressingChanged:) 

Instance Method

# onLongPressGesture(minimumDuration:maximumDistance:perform:onPressingChanged:)

Adds an action to perform when this view recognizes a long press gesture.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+visionOSwatchOS 6.0+

``` source
nonisolated
func onLongPressGesture(
    minimumDuration: Double = 0.5,
    maximumDistance: CGFloat = 10,
    perform action: @escaping () -> Void,
    onPressingChanged: ((Bool) -> Void)? = nil
) -> some View
```

## Parameters 

`minimumDuration`  

The minimum duration of the long press that must elapse before the gesture succeeds.

`maximumDistance`  

The maximum distance that the fingers or cursor performing the long press can move before the gesture fails.

`action`  

The action to perform when a long press is recognized.

`onPressingChanged`  

A closure to run when the pressing state of the gesture changes, passing the current state as a parameter.

