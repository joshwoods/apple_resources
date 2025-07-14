

- RealityKit
- RealityRenderer
- RealityRenderer.CameraOutput
-  RealityRenderer.CameraOutput.RelativeViewport 

Structure

# RealityRenderer.CameraOutput.RelativeViewport

Structure defining a viewport for rendering with a camera.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct RelativeViewport
```

## Overview

The units are relative to output texture size. To map normalized-device coordinates to the whole texture:

```
viewport = RealityRenderer.CameraOutput.RelativeViewport(originX: 0.0, originY: 0.0, width: 1.0, height: 1.0)
```

Assigning values more than 1.0 to width or height stretches the viewport in horizontal and vertical directions.

Assigning values less than 0.0 to originX or originY shifts the viewport into negative X and negative Y directions.

## Topics

### Initializers

init(originX: Double, originY: Double, width: Double, height: Double)

### Instance Properties

var height: Double

var originX: Double

var originY: Double

var width: Double

