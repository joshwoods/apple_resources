

- PencilKit
- PKStrokeReference
-  init(ink:strokePath:transform:mask:) 

Initializer

# init(ink:strokePath:transform:mask:)

Creates a stroke with the line properties, path, transform, and mask that you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

**macOS**

``` source
init(
    ink: PKInk,
    strokePath: PKStrokePath,
    transform: CGAffineTransform,
    mask: NSBezierPath?
)
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
init(
    ink: PKInk,
    strokePath: PKStrokePath,
    transform: CGAffineTransform,
    mask: UIBezierPath?
)
```

## Parameters 

`ink`  

The PKInkReference the class uses to render this stroke.

`strokePath`  

The B-spline path that describes this stroke.

`transform`  

The CGAffineTransform to apply to this stroke. Defaults to CGAffineTransformIdentity.

`mask`  

The pretransform mask the class uses to clip the rendering of the stroke.

## See Also

### Creating a stroke object

init(ink: PKInk, strokePath: PKStrokePath, transform: CGAffineTransform, mask: UIBezierPath?, randomSeed: UInt32)

Creates a stroke with the line properties, path, transform, mask, and random seed that you specify.

