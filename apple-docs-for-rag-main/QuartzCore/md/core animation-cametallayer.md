

- Core Animation
-  CAMetalLayer 

Class

# CAMetalLayer

A Core Animation layer that Metal can render into, typically displayed onscreen.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class CAMetalLayer
```

## Overview

Use a CAMetalLayer when you want to use Metal to render a layer’s contents; for example, to render into a view. Consider using MTKView instead, because this class automatically wraps a CAMetalLayer object and provides a higher-level abstraction.

If you’re using UIKit, to create a view that uses a CAMetalLayer, create a subclass of UIView and override its layerClass class method to return a CAMetalLayer:

```
+ (Class) layerClass
{
    return [CAMetalLayer class];
}
```

If you’re using AppKit, configure an NSView object to use a backing layer and assign a CAMetalLayer object to the view:

```
myView.wantsLayer = YES;
myView.layer = [CAMetalLayer layer];
```

Adjust the layer’s properties to configure its underlying pixel format and other display behaviors.

### Rendering the Layer’s Contents

A CAMetalLayer creates a pool of Metal drawable objects (CAMetalDrawable). At any given time, one of these drawable objects contains the contents of the layer. To change the layer’s contents, ask the layer for a drawable object, render into it, and then update the layer’s contents to point to the new drawable.

Call the layer’s nextDrawable() method to obtain a drawable object. Get the drawable object’s texture and create a render pass that renders to that texture, as shown in the code below:

```
CAMetalLayer *metalLayer = (CAMetalLayer*)self.layer;
id *drawable = [metalLayer nextDrawable];

MTLRenderPassDescriptor *renderPassDescriptor
                               = [MTLRenderPassDescriptor renderPassDescriptor];

renderPassDescriptor.colorAttachments[0].texture = drawable.texture;
renderPassDescriptor.colorAttachments[0].loadAction = MTLLoadActionClear;
renderPassDescriptor.colorAttachments[0].clearColor = MTLClearColorMake(0.0,0.0,0.0,1.0);
...
```

To change the layer’s contents to the new drawable, call the present(_:) method (or one of its variants) on the command buffer containing the encoded render pass, passing in the drawable object to present.

```
[commandBuffer presentDrawable:drawable];
```

### Keeping References to Drawables

The layer reuses a drawable only if it isn’t onscreen and there are no strong references to it. Further, if a drawable isn’t available when you call nextDrawable(), the system waits for one to become available. To avoid stalls in your app, request a new drawable only when you need it, and release any references to it as quickly as possible after you’re done with it.

For example, before retrieving a new drawable, you might perform other work on the CPU or submit commands to the GPU that don’t require the drawable. Then, obtain the drawable and encode a command buffer to render into it, as described above. After you commit this command buffer, release all strong references to the drawable. If you don’t release drawables correctly, the layer runs out of drawables, and future calls to nextDrawable() return `nil`.

### Releasing the Drawable

Don’t release the drawable explicitly; instead, embed your render loop within an autorelease pool block:

- Swift
- Objective-C

```
func draw(in view: MTKView) {
    autoreleasepool {
        render(view: view)
    }
}
```

```
- (void)drawInMTKView:(MTKView *)view {
    @autoreleasepool {
        [self render:view];
    }
}
```

This block releases drawables promptly and avoids possible deadlock situations with multiple drawables. Release drawables as soon as possible after committing your onscreen render pass.

Note

As of iOS 10 and tvOS 10, you can safely retain a drawable to query its properties, such as drawableID and presentedTime, after the system has presented it. If you don’t need to query these properties, release the drawable when you no longer need it.

## Topics

### Configuring the Metal Device

var device: (any MTLDevice)?

The Metal device responsible for the layer’s drawable resources.

var preferredDevice: (any MTLDevice)?

The device object that the system recommends using for this layer.

### Configuring the Layer’s Drawable Objects

var pixelFormat: MTLPixelFormat

The pixel format of the layer’s textures.

var colorspace: CGColorSpace?

The color space of the rendered content.

var framebufferOnly: Bool

A Boolean value that determines whether the layer’s textures are used only for rendering.

var drawableSize: CGSize

The size, in pixels, of textures for rendering layer content.

### Configuring Presentation Behavior

var presentsWithTransaction: Bool

A Boolean value that determines whether the layer presents its content using a Core Animation transaction.

var displaySyncEnabled: Bool

A Boolean value that determines whether the layer synchronizes its updates to the display’s refresh rate.

### Configuring Extended Dynamic Range Behavior

var wantsExtendedDynamicRangeContent: Bool

Enables extended dynamic range values onscreen.

var edrMetadata: CAEDRMetadata?

Metadata describing the tone mapping to apply to the extended dynamic range (EDR) values in the layer.

### Obtaining a Metal Drawable

func nextDrawable() -> (any CAMetalDrawable)?

Waits until a Metal drawable is available, and then returns it.

var maximumDrawableCount: Int

The number of Metal drawables in the resource pool managed by Core Animation.

var allowsNextDrawableTimeout: Bool

A Boolean value that determines whether requests for a new buffer expire if the system can’t satisfy them.

### Configuring the Metal Performance HUD

var developerHUDProperties: [AnyHashable : Any]?

The properties of the Metal performance heads-up display.

## Relationships

### Inherits From

- CALayer

### Conforms To

- CAMediaTiming
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Metal and OpenGL

protocol CAMetalDrawable

A Metal drawable associated with a Core Animation layer.

class CAEAGLLayer

A layer that supports drawing OpenGL content in iOS and tvOS applications.

Deprecated

class CAEDRMetadata

Metadata describing how extended dynamic range (EDR) values should be tone mapped.

class CAOpenGLLayer

A layer that provides a layer suitable for rendering OpenGL content.

Deprecated

class CARenderer

A layer that allows an application to render a layer tree into a Core OpenGL context.

