

- Metal
-  MTLCaptureDestination 

Enumeration

# MTLCaptureDestination

The kinds of destinations for captured command data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
enum MTLCaptureDestination
```

## Topics

### Choosing a Destination

case developerTools

An option specifying that data should be captured to Xcode and that execution should stop in Xcode after the data is captured.

case gpuTraceDocument

An option specifying that the captured command data should be saved to a GPU trace document.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Frame Capture

class MTLCaptureDescriptor

A configuration for a Metal capture session.

class MTLCaptureManager

An instance you use to capture Metal command data in your app.

protocol MTLCaptureScope

A protocol that defines custom boundaries for a GPU frame capture.

