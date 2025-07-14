

- UIKit
- UIDropSession
-  progressIndicatorStyle 

Instance Property

# progressIndicatorStyle

The drop-progress indicator style associated with the drop session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var progressIndicatorStyle: UIDropSessionProgressIndicatorStyle { get set }
```

**Required**

## Discussion

This property determines the type of progress indicator displayed when the drop operation takes a significant amount of time. The UIDropSessionProgressIndicatorStyle.default style indicates that a progress indicator is shown by the system. If you prefer to show your own progress indicator, set this property to UIDropSessionProgressIndicatorStyle.none.

