

- Metal
-  MTLCommandBufferErrorOption 

Structure

# MTLCommandBufferErrorOption

Options for reporting errors from a command buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
struct MTLCommandBufferErrorOption
```

## Topics

### Buffer Error Options

static var encoderExecutionStatus: MTLCommandBufferErrorOption

An option that instructs a command buffer to save additional details about a GPU runtime error.

### Protocol Support

init(rawValue: UInt)

Creates a set of error options from a raw integer value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Configuring the Command Buffer

var logState: (any MTLLogState)?

The shader logging configuration that the command buffer uses.

var retainedReferences: Bool

A Boolean value that indicates whether the command buffer the descriptor creates maintains strong references to the resources it uses.

var errorOptions: MTLCommandBufferErrorOption

The reporting configuration that indicates which information the GPU driver stores in a command buffer’s error property.

