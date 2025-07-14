

- SpriteKit
- SKRenderer
-  init(device:) 

Initializer

# init(device:)

Initializes with a specific GPU to render into.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init(device: any MTLDevice)
```

## Parameters 

`device`  

A Metal device.

## Return Value

A new renderer object.

## Discussion

Pass in the same Metal device that is associated to the Metal command buffer passed into render(withViewport:commandBuffer:renderPassDescriptor:).

## See Also

### First Steps

var scene: SKScene?

The scene this renderer will draw into the Metal command buffer.

