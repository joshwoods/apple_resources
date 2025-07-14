

- os
- OSAllocatedUnfairLock
-  init(initialState:) 

Initializer

# init(initialState:)

Creates a lock object that maintains and protects state data.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(initialState: State)
```

Available when `State` conforms to `Sendable`.

## Parameters 

`initialState`  

The starting state of the operation.

## See Also

### Creating a lock object

init()

Creates a lock object that doesn’t protect state data.

