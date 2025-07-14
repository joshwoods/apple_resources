

- ARKit
-  ARMatteGenerator 

Class

# ARMatteGenerator

An object that creates matte textures you use to occlude your app’s virtual content with people, that ARKit recognizes in the camera feed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARMatteGenerator
```

## Overview

Use this class when you want full control over occluding your app’s virtual content, based on people ARKit recognizes in the camera feed.

Note

Apps using one of the standard renderers (`ARView` or ARSCNView) don’t need this class to effect people occlusion. See frameSemantics for more information.

To assist your custom renderer with people occlusion, matte generator processes alpha and depth information in a frame’s segmentationBuffer and estimatedDepthData to provide you with matte and depth textures. You use these textures to layer people on top of your app’s virtual content.

## Topics

### Creating a Matte Generator

init(device: any MTLDevice, matteResolution: ARMatteGenerator.Resolution)

Creates an AR matte generator.

### Creating an Alpha Matte Texture

func generateMatte(from: ARFrame, commandBuffer: any MTLCommandBuffer) -> any MTLTexture

Generates alpha matte at either full resolution or half the resolution of the captured image.

### Creating a Depth Texture

func generateDilatedDepth(from: ARFrame, commandBuffer: any MTLCommandBuffer) -> any MTLTexture

Generates dilated depth at the resolution of the segmentation stencil.

### Controlling Resolution

enum Resolution

A resolution for a matte texture.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Occlusion

Occluding virtual content with people

Cover your app’s virtual content with people that ARKit perceives in the camera feed.

Effecting People Occlusion in Custom Renderers

Occlude your app’s virtual content where ARKit recognizes people in the camera feed by using matte generator.

Visualizing and interacting with a reconstructed scene

Estimate the shape of the physical environment using a polygonal mesh.

