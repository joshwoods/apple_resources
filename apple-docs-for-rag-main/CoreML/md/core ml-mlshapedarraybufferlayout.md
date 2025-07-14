

- Core ML
-  MLShapedArrayBufferLayout 

Enumeration

# MLShapedArrayBufferLayout

Buffer layout enum

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum MLShapedArrayBufferLayout
```

## Topics

### Enumeration Cases

case firstMajorContiguous

Layout scalars contiguously in first-major order.

case lastMajorContiguous

Layout scalars contiguously in last-major order.

case strides([Int])

Layout scalars according to the strides.

## Relationships

### Conforms To

- Sendable

