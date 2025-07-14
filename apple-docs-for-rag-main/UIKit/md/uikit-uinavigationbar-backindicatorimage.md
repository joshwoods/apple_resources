

- UIKit
- UINavigationBar
-  backIndicatorImage 

Instance Property

# backIndicatorImage

The image shown beside the Back button.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var backIndicatorImage: UIImage? { get set }
```

## Discussion

If you want to customize the back-indicator image, you must also set backIndicatorTransitionMaskImage.

## See Also

### Configuring the Back button

var backIndicatorTransitionMaskImage: UIImage?

The image used as a mask for content during push and pop transitions.

