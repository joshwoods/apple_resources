

- AppKit
- NSResponder
-  shouldBeTreatedAsInkEvent(\_:) 

Instance Method

# shouldBeTreatedAsInkEvent(\_:)

Indicates whether a pen-down event should be treated as an ink event.

macOS

``` source
@MainActor
func shouldBeTreatedAsInkEvent(_ event: NSEvent) -> Bool
```

## Parameters 

`event`  

An event object representing the event to be tested.

## Return Value

Returns true if the specified event should be treated as an ink event, false if it should be treated as a mouse event.

## Discussion

This method provides the ability to distinguish when a pen-down event should start inking versus when a pen-down event should be treated as a mouse-down event. This allows for a write-anywhere model for pen-based input.

The default implementation in NSApplication sends the method to the NSWindow object under the pen. If the window is inactive, this method returns true, unless the pen-down is in the window drag region. If the window is active, this method is sent to the NSView object under the pen.

The default implementation in NSView returns true, and NSControl overrides and returns false. This allows write-anywhere over most `NSView` objects, but allows the pen to be used to track in controls and to move windows.

A custom view should override this method to get the correct behavior for a pen-down in the view.

