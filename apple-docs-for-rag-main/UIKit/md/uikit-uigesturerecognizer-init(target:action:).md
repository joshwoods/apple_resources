

- UIKit
- UIGestureRecognizer
-  init(target:action:) 

Initializer

# init(target:action:)

Creates a gesture recognizer with a target and an action selector.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    target: Any?,
    action: Selector?
)
```

## Parameters 

`target`  

An object that is the recipient of action messages sent by the receiver when it recognizes a gesture. `nil` isn’t a valid value.

`action`  

A selector that identifies the method implemented by the target to handle the gesture recognized by the receiver. The action selector must conform to the signature described in the class overview. `nil` isn’t a valid value.

## Return Value

An initialized instance of a concrete UIGestureRecognizer subclass.

## Discussion

This method is the designated initializer. After creating the gesture recognizer, you may associate other target-action pairs with it by calling addTarget(_:action:).

## See Also

### Related Documentation

func removeTarget(Any?, action: Selector?)

Removes a target and an action from a gesture-recognizer object.

func addTarget(Any, action: Selector)

Adds a target and an action to a gesture-recognizer object.

### Initializing a gesture recognizer

convenience init?(coder: NSCoder)

Creates a gesture recognizer from data in an unarchiver.

convenience init()

Creates a gesture recognizer.

