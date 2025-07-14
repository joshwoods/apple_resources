

- ARKit
- ARConfiguration
-  ARConfiguration.FrameSemantics 

Structure

# ARConfiguration.FrameSemantics

Types of optional frame features you can enable in your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
struct FrameSemantics
```

## Discussion

A frame semantic represents 2D information that ARKit extracts from a frame.

## Topics

### Creating a Feature

init(rawValue: UInt)

Creates a frame semantics feature.

### Tracking Bodies in 2D

static var bodyDetection: ARConfiguration.FrameSemantics

An option that indicates that 2D body detection is enabled.

### Occluding Virtual Content with People

static var personSegmentation: ARConfiguration.FrameSemantics

An option that indicates that people occlude your app’s virtual content.

static var personSegmentationWithDepth: ARConfiguration.FrameSemantics

An option that indicates that people occlude your app’s virtual content depending on depth.

### Accessing Depth

static var sceneDepth: ARConfiguration.FrameSemantics

An option that provides the distance from the device to real-world objects viewed through the camera.

static var smoothedSceneDepth: ARConfiguration.FrameSemantics

An option that provides the distance from the device to real-world objects, averaged across several frames.

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

### Enabling frame features

var frameSemantics: ARConfiguration.FrameSemantics

The set of active semantics on the frame.

class func supportsFrameSemantics(ARConfiguration.FrameSemantics) -> Bool

Checks whether a particular feature is supported.

