

- AppKit
- NSResponder
-  tryToPerform(\_:with:) 

Instance Method

# tryToPerform(\_:with:)

Attempts to perform the method indicated by an action with a specified argument.

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

The selector identifying the action method.

`object`  

The object to use as the sole argument of the action method.

## Return Value

Returns false if no responder is found that responds to `action;` otherwise, true.

## Discussion

If the receiver responds to `action`, it invokes the method with `object` as the argument and returns true. If the receiver doesn’t respond, it sends this message to its next responder with the same selector and object.

## See Also

### Related Documentation

func sendAction(Selector, to: Any?, from: Any?) -> Bool

Sends the given action message to the given target.

