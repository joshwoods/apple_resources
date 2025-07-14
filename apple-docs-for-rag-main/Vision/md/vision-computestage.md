

- Vision
-  ComputeStage 

Enumeration

# ComputeStage

Types that represent the compute stage.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum ComputeStage
```

## Overview

The main compute stage represents the essential functionality of a request. Requests that provide additional analysis — or conversion of the data by the main stage — can also report a post-processing stage.

## Topics

### Getting the compute stages

case main

A stage that represents where the system performs the main functionality.

case postProcessing

A stage that represents where the system performs additional analysis after the main compute stage.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Utilities

class VideoProcessor

An object that performs offline analysis of video content.

