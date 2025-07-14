

- PencilKit
- PKStrokeReference
-  init(ink:strokePath:transform:mask:randomSeed:) 

Initializer

# init(ink:strokePath:transform:mask:randomSeed:)

Creates a stroke with the line properties, path, transform, mask, and random seed that you specify.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
init(
    ink: PKInk,
    strokePath: PKStrokePath,
    transform: CGAffineTransform,
    mask: UIBezierPath?,
    randomSeed: UInt32
)
```

**macOS**

``` source
init(
    ink: PKInk,
    strokePath: PKStrokePath,
    transform: CGAffineTransform,
    mask: NSBezierPath?,
    randomSeed: UInt32
)
```

## Parameters 

`ink`  

The PKInkReference used to render this stroke.

`strokePath`  

The B-spline path that describes this stroke.

`transform`  

The CGAffineTransform to apply to this stroke. Defaults to CGAffineTransformIdentity.

`mask`  

The pretransform mask used to clip the rendering of the stroke.

`randomSeed`  

The random seed for the stroke.

## See Also

### Creating a stroke object

init(ink: PKInk, strokePath: PKStrokePath, transform: CGAffineTransform, mask: UIBezierPath?)

Creates a stroke with the line properties, path, transform, and mask that you specify.

