

- Metal
- MTLCommandBufferEncoderInfo
-  label 

Instance Property

# label

The name of the encoder that generates the error information.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var label: String { get }
```

**Required**

## Discussion

Metal assigns the value of the property to the encoder’s label property.

## See Also

### Inspecting Execution Information

var debugSignposts: [String]

An array of debug signposts that Metal records as the GPU executes the commands of the encoder’s pass.

**Required**

var errorState: MTLCommandEncoderErrorState

The execution status of the command encoder.

**Required**

enum MTLCommandEncoderErrorState

Possible error conditions for the command encoder’s commands.

