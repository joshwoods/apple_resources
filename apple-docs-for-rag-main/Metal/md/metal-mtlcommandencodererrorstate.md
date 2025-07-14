

- Metal
-  MTLCommandEncoderErrorState 

Enumeration

# MTLCommandEncoderErrorState

Possible error conditions for the command encoder’s commands.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MTLCommandEncoderErrorState
```

## Topics

### Getting the Error State

case completed

A state that indicates the GPU successfully executed the commands without any errors.

case pending

An error state that indicates the GPU didn’t execute the commands.

case affected

An error state that indicates the GPU failed to fully execute the commands because of an error.

case faulted

An error state that indicates the commands in the command buffer are the cause of an error.

case unknown

An error state that indicates the command buffer doesn’t know the state of its commands on the GPU.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting Execution Information

var label: String

The name of the encoder that generates the error information.

**Required**

var debugSignposts: [String]

An array of debug signposts that Metal records as the GPU executes the commands of the encoder’s pass.

**Required**

var errorState: MTLCommandEncoderErrorState

The execution status of the command encoder.

**Required**

