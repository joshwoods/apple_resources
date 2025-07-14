

- Metal
-  MTLMutability 

Enumeration

# MTLMutability

The options that determine the mutability of a buffer’s contents.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum MTLMutability
```

## Topics

### Enumeration Cases

case `default`

The default behavior, based on the buffer’s type.

case mutable

An option that states that you can modify the buffer’s contents.

case immutable

An option that states that you can’t modify the buffer’s contents.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting Buffer Mutability

var mutability: MTLMutability

A mutability option that determines whether you can update a buffer’s contents before related commands use the buffer.

