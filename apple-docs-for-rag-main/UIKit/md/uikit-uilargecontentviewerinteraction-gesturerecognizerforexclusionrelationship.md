

- UIKit
- UILargeContentViewerInteraction
-  gestureRecognizerForExclusionRelationship 

Instance Property

# gestureRecognizerForExclusionRelationship

A gesture recognizer that you can use to set up simultaneous recognition or failure relationships with other gesture recognizers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var gestureRecognizerForExclusionRelationship: UIGestureRecognizer { get }
```

## See Also

### Customizing large content viewer interactions

var delegate: (any UILargeContentViewerInteractionDelegate)?

An object that can fine-tune the large content viewer interactions, especially in the presence of other gesture recognizers.

