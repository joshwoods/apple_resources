

- Metal
- MTLPipelineBufferDescriptor
-  mutability 

Instance Property

# mutability

A mutability option that determines whether you can update a buffer’s contents before related commands use the buffer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var mutability: MTLMutability { get set }
```

## Discussion

The default value is MTLMutability.default.

If you don’t explicitly declare mutability, Metal uses the following default behaviors:

- Regular buffers are mutable by default, and Metal treats MTLMutability.default as if it were MTLMutability.mutable.

- Argument buffers are immutable by default, and Metal treats MTLMutability.default as if it were MTLMutability.immutable.

## See Also

### Setting Buffer Mutability

enum MTLMutability

The options that determine the mutability of a buffer’s contents.

