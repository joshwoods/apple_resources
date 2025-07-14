

- FamilyControls
- FamilyActivityPicker
-  onLongPressGesture(minimumDuration:maximumDistance:perform:onPressingChanged:) 

Instance Method

# onLongPressGesture(minimumDuration:maximumDistance:perform:onPressingChanged:)

Adds an action to perform when this view recognizes a long press gesture.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+watchOS 6.0+

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

## See Also

### Taps and Gestures

func onTapGesture(count: Int, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a tap gesture.

func onLongPressGesture(minimumDuration: Double, perform: () -> Void, onPressingChanged: ((Bool) -> Void)?) -> some View

Adds an action to perform when this view recognizes a long press gesture.

func gesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func simultaneousGesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

