

- UIKit
- UIContentUnavailableConfiguration
- UIContentUnavailableConfiguration.ImageProperties
-  maximumSize 

Instance Property

# maximumSize

A maximum size for the image.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
var maximumSize: CGSize { get set }
```

## Discussion

The default value is CGSizeZero. Setting a width or height of zero makes the size unconstrained on that dimension. If the image exceeds maximumSize size on either dimension, the view reduces its size proportionately, maintaining aspect ratio.

