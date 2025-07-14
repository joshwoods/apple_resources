

- VisionKit
- DataScannerViewController
-  overlayContainerView 

Instance Property

# overlayContainerView

A view that the data scanner displays over its view without interfering with the Live Text interface.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
@MainActor
var overlayContainerView: UIView { get }
```

## Mentioned in 

Scanning data with the camera

## Discussion

Optionally, add custom highlights to this view that doesn’t interfere with hit-testing or the guidance objects. If you want to add interface objects above the highlights, add those objects as subviews of the view property.

## See Also

### Customizing the interface

var regionOfInterest: CGRect?

The area of the live video in view coordinates that the data scanner searches for items.

