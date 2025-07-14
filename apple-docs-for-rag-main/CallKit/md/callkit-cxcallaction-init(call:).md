

- CallKit
- CXCallAction
-  init(call:) 

Initializer

# init(call:)

Initializes a new action for a call identified by a given UUID.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
init(call callUUID: UUID)
```

## Parameters 

`callUUID`  

The unique identifier for the associated CXCall object.

## Return Value

A new action for the specified call UUID.

## See Also

### Creating New Call Actions

init?(coder: NSCoder)

Creates a new action for a call with data in an unarchiver.

