

- CallKit
- CXSetHeldCallAction
-  init(call:onHold:) 

Initializer

# init(call:onHold:)

Initializes a new action for a call identified by a given UUID, as well as whether the call is on hold.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    call callUUID: UUID,
    onHold: Bool
)
```

## Parameters 

`callUUID`  

The unique identifier for the associated CXCall object of the action.

`onHold`  

Whether the call is on hold.

## Return Value

A new action for the specified call UUID and whether the call is placed on hold.

## See Also

### Creating New Actions

init?(coder: NSCoder)

Creates a new action to place a call on hold with data in an unarchiver.

