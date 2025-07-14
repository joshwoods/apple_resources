

- UIKit
- Keyboards and input
-  Handling key presses made on a physical keyboard 

Article

# Handling key presses made on a physical keyboard

Detect when someone presses and releases keys on a physical keyboard.

## Overview

In iOS apps and Mac apps built with Mac Catalyst, the system reports key presses that a person makes on a physical keyboard by sending press events to responder objects in the responder chain of the active app.

A responder chain is a linked series of UIResponder objects, such as UIViewController and UIApplication, that either handle an event or transfer responsibility for handling the event to other responders in the app. To learn more about responders and the responder chain, see Using responders and the responder chain to handle events.

### Detect a key press

To detect a key press that a person makes on a physical keyboard, override pressesBegan(_:with:) in a responder object of your app such as the app delegate or main view controller.

To determine what key they pressed, iterate through the set of presses, inspecting the key property of each press. Use charactersIgnoringModifiers to determine the text value of key, and whether the responder should handle the key press or not. If the responder doesn’t handle the key press, call pressesBegan(_:with:) on the superclass to send the press event to the next responder in the active responder chain.

For example, the following code listing handles someone pressing either the left or right arrow.

```
// Handle someone pressing a key on a physical keyboard.
override func pressesBegan(_ presses: Set, 
                           with event: UIPressesEvent?) {

    var didHandleEvent = false

    for press in presses {

        // Get the pressed key.
        guard let key = press.key else { continue }

        if key.charactersIgnoringModifiers == UIKeyCommand.inputLeftArrow {
            // Someone pressed the left arrow key.
            // Respond to the key-press event.
            didHandleEvent = true
        }
        if key.charactersIgnoringModifiers == UIKeyCommand.inputRightArrow {
            // Someone pressed the right arrow key.
            // Respond to the key-press event.
            didHandleEvent = true
        }
    }

    if didHandleEvent == false {
        // If someone presses a key that you're not handling,
        // pass the event to the next responder.
        super.pressesBegan(presses, with: event)
    }
}
```

### Detect a key release

Override the responder’s pressesEnded(_:with:) method to detect when someone releases a key. To get information about the key, do the same as you did when detecting a key press; inspect the key property of each press in the `presses` set. For example, the following code listing handles someone releasing either the left or right arrow.

```
// Handle someone releasing a key on a physical keyboard.
override func pressesEnded(_ presses: Set, with event: UIPressesEvent?) {

    var didHandleEvent = false

    for press in presses {

        // Get the released key.
        guard let key = press.key else { continue }

        if key.charactersIgnoringModifiers == UIKeyCommand.inputLeftArrow {
            // Someone released the left arrow key.
            // Respond to the event.
            didHandleEvent = true
        }
        if key.charactersIgnoringModifiers == UIKeyCommand.inputRightArrow {
            // Someone released the right arrow key.
            // Respond to the event.
            didHandleEvent = true
        }
    }

    if didHandleEvent == false {
        // If someone releases a key that you're not handling,
        // pass the event to the next responder.
        super.pressesEnded(presses, with: event)
    }
}
```

## See Also

### Physical keyboards

Navigating an app’s user interface using a keyboard

Navigate between user interface elements using a keyboard and focusable UI elements in iPad apps and apps built with Mac Catalyst.

Adding hardware keyboard support to your app

Enhance interactions with your app by handling raw keyboard events, writing custom keyboard shortcuts, and working with gesture recognizers.

class UIKey

An object that provides information about the state of a keyboard key.

enum UIKeyboardHIDUsage

A set of HID usage codes that identify the keys of a USB keyboard.

