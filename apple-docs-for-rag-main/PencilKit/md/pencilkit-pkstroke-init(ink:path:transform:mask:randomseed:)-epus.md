

- PencilKit
- PKStroke
-  init(ink:path:transform:mask:randomSeed:) 

Initializer

# init(ink:path:transform:mask:randomSeed:)

Creates a macOS stroke with the line properties, path, transform, mask, and random seed that you specify.

iOS 16.0+iPadOS 16.0+macOS 13.0+

``` source
init(
    ink: PKInk,
    path: PKStrokePath,
    transform: CGAffineTransform = .identity,
    mask: NSBezierPath? = nil,
    randomSeed: UInt32
)
```

## Parameters 

`ink`  

The PKInkReference the framework uses to render this stroke.

`path`  

The B-spline path that describes this stroke.

`transform`  

The CGAffineTransform to apply to this stroke. Defaults to CGAffineTransformIdentity.

`mask`  

The pretransform mask the framework uses to clip the rendering of the stroke.

`randomSeed`  

The random seed for the stroke.

## See Also

### Creating a stroke object

init(ink: PKInk, path: PKStrokePath, transform: CGAffineTransform, mask: UIBezierPath?)

Creates a stroke with the line properties, path, transform, and mask that you specify.

init(ink: PKInk, path: PKStrokePath, transform: CGAffineTransform, mask: NSBezierPath?)

Creates a stroke with the line properties, path, transform, and mask that you specify.

init(ink: PKInk, path: PKStrokePath, transform: CGAffineTransform, mask: UIBezierPath?, randomSeed: UInt32)

Creates a stroke with the line properties, path, transform, mask, and random seed that you specify.

