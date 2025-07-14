

- AppKit
- NSApplication
-  tryToPerform(\_:with:) 

Instance Method

# tryToPerform(\_:with:)

Dispatches an action message to the specified target.

macOS

``` source
@MainActor
func tryToPerform(
    _ action: Selector,
    with object: Any?
) -> Bool
```

## Parameters 

`action`  

The action message you want to dispatch.

`object`  

The target object that defines the specified selector.

## Return Value

true if either the receiver or its delegate can accept the specified selector; otherwise, false. This method also returns false if `aSelector` is `nil`.

## Discussion

The receiver tries to perform the method `aSelector` using its inherited tryToPerform(_:with:) method of NSResponder. If the receiver doesn’t perform `aSelector`, the delegate is given the opportunity to perform it using its inherited perform(_:with:) method of NSObject.

## See Also

### Related Documentation

func responds(to aSelector: Selector!) -> Bool

Returns a Boolean value that indicates whether the receiver implements or inherits a method that can respond to a specified message.

### Posting Actions

func sendAction(Selector, to: Any?, from: Any?) -> Bool

Sends the given action message to the given target.

func target(forAction: Selector) -> Any?

Returns the object that receives the action message specified by the given selector.

func target(forAction: Selector, to: Any?, from: Any?) -> Any?

Searches for an object that can receive the message specified by the given selector.

