

- CallKit
- CXStartCallAction
-  init(coder:) 

Initializer

# init(coder:)

Creates a new action to start a call with data in an unarchiver.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
init?(coder aDecoder: NSCoder)
```

## Parameters 

`aDecoder`  

An unarchiver object.

## See Also

### Creating New Actions

init(call: UUID, handle: CXHandle)

Initializes a new action to start a call with the specified UUID to a recipient with the specified handle.

