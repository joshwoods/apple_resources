

- Dispatch
- DispatchSemaphore
-  init(value:) 

Initializer

# init(value:)

Creates new counting semaphore with an initial value.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(value: Int)
```

## Parameters 

`value`  

The starting value for the semaphore. Do not pass a value less than zero.

## Return Value

The newly created semaphore.

## Discussion

Passing zero for the value is useful for when two threads need to reconcile the completion of a particular event. Passing a value greater than zero is useful for managing a finite pool of resources, where the pool size is equal to the value.

Important

Calls to signal() must be balanced with calls to wait(). Attempting to dispose of a semaphore with a count lower than `value` causes an `EXC_BAD_INSTRUCTION` exception.

