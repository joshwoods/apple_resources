

- Metal
- MTLCommandBufferEncoderInfo
-  errorState 

Instance Property

# errorState

The execution status of the command encoder.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var errorState: MTLCommandEncoderErrorState { get }
```

**Required**

## See Also

### Inspecting Execution Information

var label: String

The name of the encoder that generates the error information.

**Required**

var debugSignposts: [String]

An array of debug signposts that Metal records as the GPU executes the commands of the encoder’s pass.

**Required**

enum MTLCommandEncoderErrorState

Possible error conditions for the command encoder’s commands.

