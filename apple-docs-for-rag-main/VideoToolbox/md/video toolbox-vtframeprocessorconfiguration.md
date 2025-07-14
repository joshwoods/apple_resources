

- Video Toolbox
-  VTFrameProcessorConfiguration 

Protocol

# VTFrameProcessorConfiguration

A protocol that describes the configuration of a processor to use during a video processing session.

macOS 15.4+

``` source
protocol VTFrameProcessorConfiguration : NSObjectProtocol, Sendable
```

## Overview

The VTFrameProcessorConfiguration protocol conformance starts a frame processing session. These properties can be queried on an implementation conforming to this protocol without starting a session.

## Topics

### Determining processor availability

static var processorSupported: Bool

A Boolean value that indicates whether the current configuration supports the processor.

**Required**

### Inspecting the required configuration

var frameSupportedPixelFormats: [NSNumber]

A list of supported pixel formats for the current configuration.

**Required**

var sourcePixelBufferAttributes: [AnyHashable : Any]

A dictionary of pixel buffer attributes that define what the source and reference frames passed to the processor must conform to.

**Required**

var destinationPixelBufferAttributes: [AnyHashable : Any]

A dictionary of pixel buffer attributes that define which output frames passed to the processor must conform to.

**Required**

var nextFrameCount: Int

The number of next frames that the processor requires for processing.

var previousFrameCount: Int

The number of previous frames that the processor requires for processing.

static var maximumDimensions: CMVideoDimensions

The maximum dimensions of a source frame for the processor.

static var minimumDimensions: CMVideoDimensions

The minimum dimensions of a source frame for the processor.

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

### Conforming Types

- VTFrameRateConversionConfiguration
- VTMotionBlurConfiguration
- VTOpticalFlowConfiguration

## See Also

### Frame processor

class VTFrameProcessor

A class that creates a new frame processor for the configured video effect.

class VTFrameProcessorFrame

An object that wraps video frames to send to the processor, as source, reference, or output frames.

protocol VTFrameProcessorParameters

The base protocol for input and output processing parameters for a frame processor implementation.

