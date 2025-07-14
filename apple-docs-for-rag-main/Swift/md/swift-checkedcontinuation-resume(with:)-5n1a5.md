

- Swift
- CheckedContinuation
-  resume(with:) 

Instance Method

# resume(with:)

Resume the task awaiting the continuation by having it either return normally or throw an error based on the state of the given `Result` value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func resume(with result: sending Result) where E == any Error, Er : Error
```

Available when `E` conforms to `Error`.

## Parameters 

`result`  

A value to either return or throw from the continuation.

## Discussion

A continuation must be resumed exactly once. If the continuation has already been resumed through this object, then the attempt to resume the continuation will trap.

After `resume` enqueues the task, control immediately returns to the caller. The task continues executing when its executor is able to reschedule it.

