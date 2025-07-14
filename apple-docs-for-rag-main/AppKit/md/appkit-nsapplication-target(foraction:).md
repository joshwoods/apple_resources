

- AppKit
- NSApplication
-  target(forAction:) 

Instance Method

# target(forAction:)

Returns the object that receives the action message specified by the given selector.

macOS

``` source
@MainActor
func target(forAction action: Selector) -> Any?
```

## Parameters 

`action`  

The desired action message.

## Return Value

The object that would receive the specified action message or `nil` if no target object would receive the message. This method also returns `nil` if `aSelector` is `nil`.

## See Also

### Posting Actions

func tryToPerform(Selector, with: Any?) -> Bool

Dispatches an action message to the specified target.

func sendAction(Selector, to: Any?, from: Any?) -> Bool

Sends the given action message to the given target.

func target(forAction: Selector, to: Any?, from: Any?) -> Any?

Searches for an object that can receive the message specified by the given selector.

