

- AppKit
- NSGestureRecognizerDelegate
-  gestureRecognizer(\_:shouldReceive:) 

Instance Method

# gestureRecognizer(\_:shouldReceive:)

Called, for a new touch, before the system calls the `touchesBegan:withEvent:` method on the gesture recognizer. Return `NO` to prevent the gesture recognizer from seeing this touch.

macOS 10.12.2+

``` source
@MainActor
optional func gestureRecognizer(
    _ gestureRecognizer: NSGestureRecognizer,
    shouldReceive touch: NSTouch
) -> Bool
```

