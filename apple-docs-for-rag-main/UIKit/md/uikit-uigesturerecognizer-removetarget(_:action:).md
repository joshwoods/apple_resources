

- UIKit
- UIGestureRecognizer
-  removeTarget(\_:action:) 

Instance Method

# removeTarget(\_:action:)

Removes a target and an action from a gesture-recognizer object.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func removeTarget(
    _ target: Any?,
    action: Selector?
)
```

## Parameters 

`target`  

An object that currently is a recipient of action messages sent by the receiver when the represented gesture occurs. Specify `nil` if you want to remove all targets from the receiver.

`action`  

A selector identifying a method of a target to be invoked by the action message. Specify `NULL` if you want to remove all actions from the receiver.

## Discussion

Calling this method removes the specified target-action pair. Passing `nil` for `target` matches all targets and passing `NULL` for `action` matches all actions.

## See Also

### Related Documentation

init(target: Any?, action: Selector?)

Creates a gesture recognizer with a target and an action selector.

### Adding and removing targets and actions

func addTarget(Any, action: Selector)

Adds a target and an action to a gesture-recognizer object.

