

- UIKit
- UIButton
- UIButton.Configuration
-  showsActivityIndicator 

Instance Property

# showsActivityIndicator

A Boolean value that determines whether the button displays an activity indicator instead of an image.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var showsActivityIndicator: Bool { get set }
```

## Discussion

The button respects the imagePlacement property when positioning the activity indicator.

## See Also

### Configuring the activity indicator

var activityIndicatorColorTransformer: UIConfigurationColorTransformer?

The color transformer for resolving the color of the activity indicator.

