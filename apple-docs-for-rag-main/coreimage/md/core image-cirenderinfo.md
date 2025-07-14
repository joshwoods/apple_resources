

- Core Image
-  CIRenderInfo 

Class

# CIRenderInfo

An encapsulation of a render task's timing, passes, and pixels processed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class CIRenderInfo : NSObject
```

## Overview

A `CIRenderInfo` object allows Xcode Quick Look to visualize the render graph with detailed timing information.

## Topics

### Instance Properties

var kernelExecutionTime: TimeInterval

The amount of time a render spent executing kernels.

var passCount: Int

The number of passes the render took.

var pixelsProcessed: Int

The number of pixels the render produced executing kernels.

var kernelCompileTime: TimeInterval

## Relationships

### Inherits From

- NSObject

## See Also

### Custom Render Destination

Generating an animation with a Core Image Render Destination

Animate a filtered image to a Metal view in a SwiftUI app using a Core Image Render Destination.

class CIRenderDestination

A specification for configuring all attributes of a render task's destination and issuing asynchronous render tasks.

class CIRenderTask

A single render task issued in conjunction with CIRenderDestination.

enum CIRenderDestinationAlphaMode

Different ways of representing alpha.

