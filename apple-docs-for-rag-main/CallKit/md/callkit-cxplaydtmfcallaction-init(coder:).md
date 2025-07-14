

- CallKit
- CXPlayDTMFCallAction
-  init(coder:) 

Initializer

# init(coder:)

Creates a new action to play dual-tone multifrequency (DTMF) tones with data in an unarchiver.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
init?(coder aDecoder: NSCoder)
```

## Parameters 

`aDecoder`  

An unarchiver object.

## See Also

### Creating New Actions

init(call: UUID, digits: String, type: CXPlayDTMFCallAction.ActionType)

Initializes a new action for a call identified by a given UUID, as well as a specified type and sequence of digits.

