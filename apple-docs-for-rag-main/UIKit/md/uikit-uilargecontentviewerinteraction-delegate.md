

- UIKit
- UILargeContentViewerInteraction
-  delegate 

Instance Property

# delegate

An object that can fine-tune the large content viewer interactions, especially in the presence of other gesture recognizers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UILargeContentViewerInteractionDelegate)? { get }
```

## See Also

### Customizing large content viewer interactions

var gestureRecognizerForExclusionRelationship: UIGestureRecognizer

A gesture recognizer that you can use to set up simultaneous recognition or failure relationships with other gesture recognizers.

