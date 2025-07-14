

- UIKit
- UIControl
- UIControl.Event
-  touchDragOutside 

Type Property

# touchDragOutside

An event where a finger is dragged just outside the bounds of the control.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
static var touchDragOutside: UIControl.Event { get }
```

## See Also

### Constants

static var touchDown: UIControl.Event

A touch-down event in the control.

static var touchDownRepeat: UIControl.Event

A repeated touch-down event in the control; for this event the value of the UITouch `tapCount` method is greater than one.

static var touchDragInside: UIControl.Event

An event where a finger is dragged inside the bounds of the control.

static var touchDragEnter: UIControl.Event

An event where a finger is dragged into the bounds of the control.

static var touchDragExit: UIControl.Event

An event where a finger is dragged from within a control to outside its bounds.

static var touchUpInside: UIControl.Event

A touch-up event in the control where the finger is inside the bounds of the control.

static var touchUpOutside: UIControl.Event

A touch-up event in the control where the finger is outside the bounds of the control.

static var touchCancel: UIControl.Event

A system event canceling the current touches for the control.

static var valueChanged: UIControl.Event

A touch dragging or otherwise manipulating a control, causing it to emit a series of different values.

static var menuActionTriggered: UIControl.Event

A menu action has triggered prior to the menu being presented.

static var primaryActionTriggered: UIControl.Event

A semantic action triggered by buttons.

static var editingDidBegin: UIControl.Event

A touch initiating an editing session in a text field by entering its bounds.

static var editingChanged: UIControl.Event

A touch making an editing change in a text field.

static var editingDidEnd: UIControl.Event

A touch ending an editing session in a text field by leaving its bounds.

static var editingDidEndOnExit: UIControl.Event

A touch ending an editing session in a text field.

