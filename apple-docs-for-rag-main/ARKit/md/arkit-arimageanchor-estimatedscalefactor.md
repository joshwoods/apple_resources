

- ARKit
- ARImageAnchor
-  estimatedScaleFactor 

Instance Property

# estimatedScaleFactor

A factor between the initial size and the estimated physical size.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var estimatedScaleFactor: CGFloat { get }
```

## Discussion

The default value is 1.0, which means that a version of this image that ARKit recognizes in the physical environment exactly matches its reference image physicalSize.

Otherwise, ARKit automatically corrects the image anchor’s transform when `estimatedScaleFactor` is a value other than 1.0. This adjustment in turn, corrects ARKit’s understanding of where the image anchor is located in the physical environment.

See automaticImageScaleEstimationEnabled.

