

- SceneKit
- SCNMaterialProperty
-  contents 

Instance Property

# contents

The visual contents of the material property—a color, image, or source of animated content. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var contents: Any? { get set }
```

## Discussion

For details on each visual property and the ways their contents affect a material’s appearance, see SCNMaterial.

You can set a value for this property using any of the following types:

- A color (NSColor/UIColor or CGColor), specifying a uniform color for the material’s surface

- A number (NSNumber), specifying a uniform scalar value for the material’s surface (useful for physically based properties such as metalness)

- An image (NSImage/UIImage or CGImage), specifying a texture to be mapped across the material’s surface

- An NSString or NSURL object specifying the location of an image file

- A video player (AVPlayer) or live video capture preview (AVCaptureDevice, in iOS only)

- A Core Animation layer (CALayer)

- A texture (SKTexture, MDLTexture, MTLTexture, or GLKTextureInfo)

- A SpriteKit scene (SKScene)

- A specially formatted image or array of six images, specifying the faces of a cube map

When you examine elements of a scene loaded from a file, this value is always either a color object (of the NSColor or UIColor class, according to platform) or an image object (of the NSImage or UIImage class, according to platform). You can therefore use type introspection (the isKind(of:) method in Objective-C, or the `is` operator or `let`-`as` matching in Swift) to determine the type of the material property’s contents.

### Using Animated Content

In iOS 11, you may use an AVCaptureDevice object to preview live video from a capture device as a material property. In iOS 11, tvOS 11, and macOS 10.13, you may use an AVPlayer object as a material property for video playback.

You may specify any Core Animation layer as the contents of a material property, such as a layer with an animated sublayer hierarchy. SceneKit cannot use a layer that is already being displayed elsewhere (for example, the backing layer of a UIView object).

You can use the SpriteKit framework to provide static or animated content for a material property. SpriteKit provides options for generating and modifying texture images, such as the generatingNormalMap() method. You can also use an entire animated SpriteKit scene as the material property’s contents. When you use a SKTexture object as a material property’s contents, the wrapS, wrapT, contentsTransform, minificationFilter, magnificationFilter and mipFilter properties automatically update to match the corresponding features of the SpriteKit texture.

If the current content is a solid color, you can use explicit or implicit animations (see Animating SceneKit Content) to change to another color, creating an effect that fades between the two colors. Using animations to change from or to other content types results in an instantaneous transition—for an animated transition between textured content types (or types that are themselves animated), create a shader modifier (see SCNShadable).

### Using Cube Map Texures

SceneKit supports cube maps only for a material’s reflective property or for a scene’s background or lightingEnvironment property. You can provide a cube map in any of the ways described in Table 1. Of these formats, the vertical strip provides the best performance, because it matches the memory layout SceneKit uses for rendering cube textures.

| Description | Image Size Requirements | Example |
|----|----|----|
| Vertical strip (single image) | height == 6 \* width |  |
| Horizontal strip (single image) | 6 \* height == width |  |
| Spherical projection (single image)  (pixel x/y positions map to latitude/longitude coordinates on a sphere) | 2 \* height == width |  |
| Array of six images  (face order: +X, -X, +Y, -Y, +Z, -Z) | height == width  same size for all images | \[, , , , , \] |

## See Also

### Working with Material Property Contents

var intensity: CGFloat

A number between `0.0` and `1.0` that modulates the effect of the material property. Animatable.

