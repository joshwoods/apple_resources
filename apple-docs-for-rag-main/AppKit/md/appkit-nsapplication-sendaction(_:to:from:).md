

- AppKit
- NSApplication
-  sendAction(\_:to:from:) 

Instance Method

# sendAction(\_:to:from:)

Sends the given action message to the given target.

macOS

``` source
@MainActor
func sendAction(
    _ action: Selector,
    to target: Any?,
    from sender: Any?
) -> Bool
```

## Parameters 

`action`  

The action message you want to send.

`target`  

The target object that defines the specified action message.

`sender`  

The object to pass for the action message’s parameter.

## Return Value

true if the action was successfully sent; otherwise false. This method also returns false if `anAction` is `nil`.

## Discussion

If `aTarget` is `nil`, shared looks for an object that can respond to the message—that is, an object that implements a method matching `anAction`. It begins with the first responder of the key window. If the first responder can’t respond, it tries the first responder’s next responder and continues following next responder links up the responder chain. If none of the objects in the key window’s responder chain can handle the message, shared attempts to send the message to the key window’s delegate.

If the delegate doesn’t respond and the main window is different from the key window, shared begins again with the first responder in the main window. If objects in the main window can’t respond, shared attempts to send the message to the main window’s delegate. If still no object has responded, shared tries to handle the message itself. If shared can’t respond, it attempts to send the message to its own delegate.

## See Also

### Related Documentation

func makeWindowsPerform(Selector, inOrder: Bool) -> NSWindow?

Sends the specified message to each of the app’s window objects until one returns a non-`nil` value.

Deprecated

### Posting Actions

func tryToPerform(Selector, with: Any?) -> Bool

Dispatches an action message to the specified target.

func target(forAction: Selector) -> Any?

Returns the object that receives the action message specified by the given selector.

func target(forAction: Selector, to: Any?, from: Any?) -> Any?

Searches for an object that can receive the message specified by the given selector.

