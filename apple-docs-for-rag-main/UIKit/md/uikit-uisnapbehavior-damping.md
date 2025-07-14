

- UIKit
- UISnapBehavior
-  damping 

Instance Property

# damping

The amount of oscillation of a dynamic item during the conclusion of a snap.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var damping: CGFloat { get set }
```

## Discussion

The valid range for damping extends from `0.0`, for maximum oscillation, through `1.0`, for minimum oscillation. The default value is `0.5`.

## See Also

### Configuring a snap behavior

var snapPoint: CGPoint

The point to which to snap.

