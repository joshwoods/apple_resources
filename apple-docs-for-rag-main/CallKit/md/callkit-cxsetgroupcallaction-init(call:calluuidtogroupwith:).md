

- CallKit
- CXSetGroupCallAction
-  init(call:callUUIDToGroupWith:) 

Initializer

# init(call:callUUIDToGroupWith:)

Initializes a new action for a call identified by a given UUID, as well as a call to group with identified by another UUID.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    call callUUID: UUID,
    callUUIDToGroupWith: UUID?
)
```

## Parameters 

`callUUID`  

The unique identifier for the associated CXCall object of the action.

`callUUIDToGroupWith`  

The unique identifier of a CXCall object for the call associated with the action to group with.

If `nil`, the the call associated with the receiver leaves any group it’s currently a member of.

## Return Value

A new action for the specified call UUID and call UUID to group with.

## See Also

### Creating New Actions

init?(coder: NSCoder)

Creates a new action to group calls with data in an unarchiver.

