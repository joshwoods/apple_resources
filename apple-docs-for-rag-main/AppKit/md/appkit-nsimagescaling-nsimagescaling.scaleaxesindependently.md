

- AppKit
- NSImageScaling
-  NSImageScaling.scaleAxesIndependently 

Case

# NSImageScaling.scaleAxesIndependently

Scale each dimension to exactly fit destination.

macOS 10.5+

``` source
case scaleAxesIndependently
```

## Discussion

This setting does not preserve the aspect ratio of the image.

## See Also

### Constants

case scaleProportionallyDown

If it is too large for the destination, scale the image down while preserving the aspect ratio.

case scaleNone

Do not scale the image.

case scaleProportionallyUpOrDown

Scale the image to its maximum possible dimensions while both staying within the destination area and preserving its aspect ratio.

