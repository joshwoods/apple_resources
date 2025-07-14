

- UIKit
- UITraitCollection
-  displayScale 

Instance Property

# displayScale

The display scale of the trait collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
var displayScale: CGFloat { get }
```

## Discussion

A value of `1.0` indicates a non-Retina display and a value of `2.0` indicates a Retina display. The default display scale for a trait collection is `0.0` (indicating unspecified).

## See Also

### Retrieving display-related traits

var displayGamut: UIDisplayGamut

The gamut of the current display.

enum UIDisplayGamut

Constants that indicate the gamut of the current display.

