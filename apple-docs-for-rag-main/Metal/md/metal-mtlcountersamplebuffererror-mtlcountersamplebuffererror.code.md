

- Metal
- MTLCounterSampleBufferError
-  MTLCounterSampleBufferError.Code 

Enumeration

# MTLCounterSampleBufferError.Code

The underlying error code type that indicates why a GPU driver can’t create a counter sample buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Error Codes

case outOfMemory

An error code that indicates the GPU device doesn’t have sufficient memory to create a counter sample buffer.

case invalid

An error code that indicates when a counter-sample buffer descriptor has at least one invalid property.

case `internal`

An error code that indicates the Metal framework has an internal problem.

case outOfMemory

An error code that indicates the GPU device doesn’t have sufficient memory to create a counter sample buffer.

case invalid

An error code that indicates when a counter-sample buffer descriptor has at least one invalid property.

case `internal`

An error code that indicates the Metal framework has an internal problem.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

