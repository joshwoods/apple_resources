

- Core Image
-  CIRenderTask 

Class

# CIRenderTask

A single render task issued in conjunction with CIRenderDestination.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class CIRenderTask : NSObject
```

## Overview

A `CIRenderTask` object appears in Xcode Quick Look as a graph.

## Topics

### Instance Methods

func waitUntilCompleted() -> CIRenderInfo

Waits until the CIRenderTask finishes and returns.

## Relationships

### Inherits From

- NSObject

## See Also

### Custom Render Destination

Generating an animation with a Core Image Render Destination

Animate a filtered image to a Metal view in a SwiftUI app using a Core Image Render Destination.

class CIRenderDestination

A specification for configuring all attributes of a render task's destination and issuing asynchronous render tasks.

class CIRenderInfo

An encapsulation of a render task's timing, passes, and pixels processed.

enum CIRenderDestinationAlphaMode

Different ways of representing alpha.

