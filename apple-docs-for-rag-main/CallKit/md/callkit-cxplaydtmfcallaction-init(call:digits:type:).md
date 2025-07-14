

- CallKit
- CXPlayDTMFCallAction
-  init(call:digits:type:) 

Initializer

# init(call:digits:type:)

Initializes a new action for a call identified by a given UUID, as well as a specified type and sequence of digits.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    call callUUID: UUID,
    digits: String,
    type: CXPlayDTMFCallAction.ActionType
)
```

## Parameters 

`callUUID`  

The unique identifier for the associated CXCall object.

`digits`  

A sequence of digits.

`type`  

The type of the call action. For possible values, see CXPlayDTMFCallAction.ActionType.

## Return Value

## Discussion

A new action for the specified call UUID, type, and digits.

## See Also

### Creating New Actions

init?(coder: NSCoder)

Creates a new action to play dual-tone multifrequency (DTMF) tones with data in an unarchiver.

