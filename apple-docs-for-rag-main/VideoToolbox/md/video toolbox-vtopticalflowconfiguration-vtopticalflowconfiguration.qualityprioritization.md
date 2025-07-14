

- Video Toolbox
- VTOpticalFlowConfiguration
-  VTOpticalFlowConfiguration.QualityPrioritization 

Enumeration

# VTOpticalFlowConfiguration.QualityPrioritization

Values that specify whether to prioritize quality or performance.

macOS 15.4+

``` source
enum QualityPrioritization
```

## Overview

See VEFrameRateConversionConfigurationQualityPrioritization for more info.

## Topics

### Enumeration Cases

case normal

A normal quality prioritization level.

case quality

A quality prioritization level.

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

### Inspecting the configuration

var frameWidth: Int

The width of a source frame in pixels.

var frameHeight: Int

The height of source frame in pixels.

var sourcePixelBufferAttributes: [String : any Sendable]

A dictionary of pixel buffer attributes describing requirements for pixel buffers used as source frames and reference frames.

var destinationPixelBufferAttributes: [String : any Sendable]

A dictionary of pixel buffer attributes describing the requirements for pixel buffers used as destination frames.

var frameSupportedPixelFormats: [NSNumber]

A list of source frame supported pixel formats for the current configuration.

var qualityPrioritization: VTOpticalFlowConfiguration.QualityPrioritization

A value that specifies whether to prioritize quality or performance.

