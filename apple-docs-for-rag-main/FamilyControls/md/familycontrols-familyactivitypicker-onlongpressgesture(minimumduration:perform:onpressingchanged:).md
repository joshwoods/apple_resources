

- FamilyControls
- FamilyActivityPicker
-  onLongPressGesture(minimumDuration:perform:onPressingChanged:) 

Instance Method

# onLongPressGesture(minimumDuration:perform:onPressingChanged:)

Adds an action to perform when this view recognizes a long press gesture.

FamilyControlsSwiftUItvOS 14.0+

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

## See Also

### Taps and Gestures

func onTapGesture(count: Int, perform: () -> Void) -> some View

Adds an action to perform when this view recognizes a tap gesture.

func onLongPressGesture(minimumDuration: Double, maximumDistance: CGFloat, perform: () -> Void, onPressingChanged: ((Bool) -> Void)?) -> some View

Adds an action to perform when this view recognizes a long press gesture.

func gesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view with a lower precedence than gestures defined by the view.

func highPriorityGesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view with a higher precedence than gestures defined by the view.

func simultaneousGesture&lt;T>(T, including: GestureMask) -> some View

Attaches a gesture to the view to process simultaneously with gestures defined by the view.

