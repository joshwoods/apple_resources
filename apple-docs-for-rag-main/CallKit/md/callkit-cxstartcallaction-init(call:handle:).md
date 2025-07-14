

- CallKit
- CXStartCallAction
-  init(call:handle:) 

Initializer

# init(call:handle:)

Initializes a new action to start a call with the specified UUID to a recipient with the specified handle.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    call callUUID: UUID,
    handle: CXHandle
)
```

## Parameters 

`callUUID`  

The unique identifier for the associated CXCall object.

`handle`  

The handle for the receipient, such as a phone number or email address.

## Return Value

A new action for the specified call UUID and handle.

## See Also

### Creating New Actions

init?(coder: NSCoder)

Creates a new action to start a call with data in an unarchiver.

