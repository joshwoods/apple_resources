

- AppKit
- NSWindow
-  makeFirstResponder(\_:) 

Instance Method

# makeFirstResponder(\_:)

Attempts to make a given responder the first responder for the window.

macOS

``` source
@MainActor
func makeFirstResponder(_ responder: NSResponder?) -> Bool
```

## Parameters 

`responder`  

The responder to set as the window’s first responder. `nil` makes the window its first responder.

## Return Value

true when the operation is successful; otherwise, false.

## Discussion

If `responder` isn’t already the first responder, this method first sends a resignFirstResponder() message to the object that is the first responder. If that object refuses to resign, it remains the first responder, and this method immediately returns false. If the current first responder resigns, this method sends a becomeFirstResponder() message to `responder`. If `responder` does not accept first responder status, the `NSWindow` object becomes first responder; in this case, the method returns true even if `responder` refuses first responder status.

If `responder` is `nil`, this method still sends resignFirstResponder() to the current first responder. If the current first responder refuses to resign, it remains the first responder and this method immediately returns false. If the current first responder returns true from resignFirstResponder(), the window is made its own first responder and this method returns true.

The Application Kit framework uses this method to alter the first responder in response to mouse-down events; you can also use it to explicitly set the first responder from within your program. The `responder` object is typically an `NSView` object in the window’s view hierarchy. If this method is called explicitly, first send acceptsFirstResponder to `responder`, and do not call makeFirstResponder(_:) if acceptsFirstResponder returns false.

Use initialFirstResponder to the set the first responder to be used when the window is brought onscreen for the first time.

## See Also

### Related Documentation

func becomeFirstResponder() -> Bool

Notifies the receiver that it’s about to become first responder in its NSWindow.

func resignFirstResponder() -> Bool

Notifies the receiver that it’s been asked to relinquish its status as first responder in its window.

### Managing Responders

var initialFirstResponder: NSView?

The view that’s made first responder (also called the key view) the first time the window is placed onscreen.

var firstResponder: NSResponder?

The window’s first responder.

