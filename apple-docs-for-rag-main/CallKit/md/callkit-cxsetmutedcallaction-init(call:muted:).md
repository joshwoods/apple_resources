

- CallKit
- CXSetMutedCallAction
-  init(call:muted:) 

Initializer

# init(call:muted:)

Initializes a new action for a call identified by a given UUID, as well as whether the call is muted.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init(
    call callUUID: UUID,
    muted: Bool
)
```

## Parameters 

`callUUID`  

The unique identifier for the associated CXCall object of the action.

`muted`  

Whether the call is muted.

## Return Value

A new action for the specified call UUID and whether the call is muted.

## See Also

### Creating New Actions

init?(coder: NSCoder)

Creates a new action for a call with data in an unarchiver.

