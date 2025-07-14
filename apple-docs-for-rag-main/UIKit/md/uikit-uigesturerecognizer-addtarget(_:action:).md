

- UIKit
- UIGestureRecognizer
-  addTarget(\_:action:) 

Instance Method

# addTarget(\_:action:)

Adds a target and an action to a gesture-recognizer object.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addTarget(
    _ target: Any,
    action: Selector
)
```

## Parameters 

`target`  

An object that is a recipient of action messages sent by the receiver when the represented gesture occurs. `nil` is not a valid value.

`action`  

A selector identifying a method of a target to be invoked by the action message. `NULL` is not a valid value.

## Discussion

You may call this method multiple times to specify multiple target-action pairs. However, if you request to add a target-action pair that has already been added, then the request is ignored.

## See Also

### Related Documentation

init(target: Any?, action: Selector?)

Creates a gesture recognizer with a target and an action selector.

### Adding and removing targets and actions

func removeTarget(Any?, action: Selector?)

Removes a target and an action from a gesture-recognizer object.

