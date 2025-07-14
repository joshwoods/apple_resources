

- UIKit
- UIPointerStyle
-  accessories 

Instance Property

# accessories

Accessories to display alongside the pointer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var accessories: [UIPointerAccessory] { get set }
```

## Discussion

This property supports up to four pointer accessories. The system animates between neighboring or similar accessories.

## See Also

### Specifying pointer accessories

class UIPointerAccessory

Constants that describe accessories to display alongside the primary pointer.

