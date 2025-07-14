

- SceneKit
- SCNRenderer
-  snapshot(atTime:with:antialiasingMode:) 

Instance Method

# snapshot(atTime:with:antialiasingMode:)

Creates an image by drawing the renderer’s content at the specified system time.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func snapshot(
    atTime time: CFTimeInterval,
    with size: CGSize,
    antialiasingMode: SCNAntialiasingMode
) -> UIImage
```

**macOS**

``` source
func snapshot(
    atTime time: CFTimeInterval,
    with size: CGSize,
    antialiasingMode: SCNAntialiasingMode
) -> NSImage
```

## Parameters 

`time`  

The timestamp, in seconds, at which to render the scene.

`size`  

The size, in pixels, of the image to create.

`antialiasingMode`  

The antialiasing mode to use for the image output.

## Return Value

An image object reflecting the contents of the scene.

## Discussion

When you call this method, SceneKit updates its hierarchy of presentation nodes based on the specified timestamp, and then draws the scene into a new image object of the specified size.

