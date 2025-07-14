

- Core Video
-  CVPixelBufferPoolFlushFlags 

Structure

# CVPixelBufferPoolFlushFlags

The flags to pass to flush the pool.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct CVPixelBufferPoolFlushFlags
```

## Topics

### Type Properties

static var excessBuffers: CVPixelBufferPoolFlushFlags

The value to pass to flush all unused buffers regardless of age.

### Initializers

init(rawValue: CVOptionFlags)

Creates a pixel buffer pool flush flags set with the options flags that you specify.

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

### Data types

class CVPixelBufferPool

A reference to a pixel buffer pool object.

