

- Metal
- MTLCommandEncoderErrorState
-  MTLCommandEncoderErrorState.completed 

Case

# MTLCommandEncoderErrorState.completed

A state that indicates the GPU successfully executed the commands without any errors.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
case completed
```

## See Also

### Getting the Error State

case pending

An error state that indicates the GPU didn’t execute the commands.

case affected

An error state that indicates the GPU failed to fully execute the commands because of an error.

case faulted

An error state that indicates the commands in the command buffer are the cause of an error.

case unknown

An error state that indicates the command buffer doesn’t know the state of its commands on the GPU.

