

- Metal
- MTLCounterSampleBufferError
-  internal 

Type Property

# internal

An error code that indicates the Metal framework has an internal problem.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static var `internal`: MTLCounterSampleBufferError.Code { get }
```

## Discussion

The local description contains the underlying error code. You can report the scenario that generated this error code with Feedback Assistant.

## See Also

### Error Code Values

static var outOfMemory: MTLCounterSampleBufferError.Code

An error code that indicates the GPU device doesn’t have sufficient memory to create a counter sample buffer.

static var invalid: MTLCounterSampleBufferError.Code

An error code that indicates the descriptor for creating a counter sample buffer descriptor has an invalid property.

enum Code

The underlying error code type that indicates why a GPU driver can’t create a counter sample buffer.

