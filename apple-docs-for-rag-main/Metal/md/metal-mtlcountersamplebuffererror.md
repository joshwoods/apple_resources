

- Metal
-  MTLCounterSampleBufferError 

Structure

# MTLCounterSampleBufferError

The error codes that indicate why a GPU driver can’t create a counter sample buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
struct MTLCounterSampleBufferError
```

## Topics

### Error Code Values

static var outOfMemory: MTLCounterSampleBufferError.Code

An error code that indicates the GPU device doesn’t have sufficient memory to create a counter sample buffer.

static var invalid: MTLCounterSampleBufferError.Code

An error code that indicates the descriptor for creating a counter sample buffer descriptor has an invalid property.

static var `internal`: MTLCounterSampleBufferError.Code

An error code that indicates the Metal framework has an internal problem.

enum Code

The underlying error code type that indicates why a GPU driver can’t create a counter sample buffer.

### Error Domain

static var errorDomain: String

The current counter sample buffer error domain.

let MTLCounterErrorDomain: String

The domain for Metal counter sample buffer errors.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

