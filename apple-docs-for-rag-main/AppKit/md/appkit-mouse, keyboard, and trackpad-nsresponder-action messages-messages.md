

- AppKit
- Mouse, Keyboard, and Trackpad
- NSResponder
-  Action Messages 

API Collection

# Action Messages

Implement action messages in your first responders to handle common tasks.

## Topics

### Help

func showContextHelp(Any?)

Implemented by subclasses to invoke the help system, displaying information relevant to the receiver and its current state.

## See Also

### Responding to Action Messages

func supplementalTarget(forAction: Selector, sender: Any?) -> Any?

Finds a target for an action method.

protocol NSStandardKeyBindingResponding

Methods that responder subclasses implement to support key binding commands, such as inserting tabs and newlines, or moving the insertion point.

