

- AppKit
- NSResponder
-  supplementalTarget(forAction:sender:) 

Instance Method

# supplementalTarget(forAction:sender:)

Finds a target for an action method.

macOS 10.7+

``` source
@MainActor
func supplementalTarget(
    forAction action: Selector,
    sender: Any?
) -> Any?
```

## Parameters 

`action`  

The requested action.

`sender`  

The message sender.

## Return Value

An object which responds to the action, or `nil`.

## Discussion

If this `NSResponder` instance does not itself `respondsToSelector:`, then `supplementalTargetForAction:sender:` is called.

This method should return an object which responds to the action; if this responder does not have a supplemental object that does that, the implementation of this method should call `super`’s `supplementalTargetForAction:sender:`.

NSResponder’s implementation returns `nil`.

## See Also

### Responding to Action Messages

protocol NSStandardKeyBindingResponding

Methods that responder subclasses implement to support key binding commands, such as inserting tabs and newlines, or moving the insertion point.

Action Messages

Implement action messages in your first responders to handle common tasks.

