

- Metal Performance Shaders Graph
-  MPSGraphOptions 

Enumeration

# MPSGraphOptions

The options available to a graph.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum MPSGraphOptions
```

## Topics

### Enumeration Cases

case none

No Options.

case synchronizeResults

The graph synchronizes results to the CPU using a blit encoder if on a discrete GPU at the end of execution.

case verbose

The framework prints more logging info.

### Initializers

init?(rawValue: UInt64)

### Type Properties

static var `default`: MPSGraphOptions

The framework uses these options as default if not overriden.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

