

- UIKit
- UIContentUnavailableConfiguration
- UIContentUnavailableConfiguration.ImageProperties
-  cornerRadius 

Instance Property

# cornerRadius

The preferred corner radius for the image.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
var cornerRadius: CGFloat { get set }
```

## Discussion

The default value is 0. If the image is too small to fit the requested radius, the view adjusts the corner curve and radius to fit.

