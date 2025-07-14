

- UIKit
- UIBezierPath
-  apply(\_:) 

Instance Method

# apply(\_:)

Transforms all points in the path using the specified affine transform matrix.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func apply(_ transform: CGAffineTransform)
```

## Parameters 

`transform`  

The transform matrix to apply to the path.

## Discussion

This method applies the specified transform to the path’s points immediately. The modifications made to the path object are permanent. If you do not want to permanently modify a path object, you should consider applying the transform to a copy.

