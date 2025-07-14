

- PencilKit
- PKStroke
-  init(ink:path:transform:mask:) 

Initializer

# init(ink:path:transform:mask:)

Creates a stroke with the line properties, path, transform, and mask that you specify.

iOS 14.0+iPadOS 14.0+macOS 11.0+

``` source
init(
    ink: PKInk,
    path: PKStrokePath,
    transform: CGAffineTransform = .identity,
    mask: NSBezierPath? = nil
)
```

## Parameters 

`ink`  

The PKInk the framework uses to render this stroke.

`path`  

The B-spline path that describes this stroke.

`transform`  

The CGAffineTransform to apply to this stroke.

`mask`  

The pretransform mask the framework uses to clip the rendering of the stroke.

## See Also

### Creating a stroke object

init(ink: PKInk, path: PKStrokePath, transform: CGAffineTransform, mask: UIBezierPath?)

Creates a stroke with the line properties, path, transform, and mask that you specify.

init(ink: PKInk, path: PKStrokePath, transform: CGAffineTransform, mask: UIBezierPath?, randomSeed: UInt32)

Creates a stroke with the line properties, path, transform, mask, and random seed that you specify.

init(ink: PKInk, path: PKStrokePath, transform: CGAffineTransform, mask: NSBezierPath?, randomSeed: UInt32)

Creates a macOS stroke with the line properties, path, transform, mask, and random seed that you specify.

