

- DeviceActivity
- DeviceActivityReport
-  onLongPressGesture(minimumDuration:perform:onPressingChanged:) 

Instance Method

# onLongPressGesture(minimumDuration:perform:onPressingChanged:)

Adds an action to perform when this view recognizes a long press gesture.

DeviceActivitySwiftUItvOS 14.0+

``` source
nonisolated
func onLongPressGesture(
    minimumDuration: Double = 0.5,
    perform action: @escaping () -> Void,
    onPressingChanged: ((Bool) -> Void)? = nil
) -> some View
```

## Parameters 

`minimumDuration`  

The minimum duration of the long press that must elapse before the gesture succeeds.

`action`  

The action to perform when a long press is recognized.

`onPressingChanged`  

A closure to run when the pressing state of the gesture changes, passing the current state as a parameter.

