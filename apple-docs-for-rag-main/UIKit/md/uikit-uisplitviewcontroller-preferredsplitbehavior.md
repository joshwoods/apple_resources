

- UIKit
- UISplitViewController
-  preferredSplitBehavior 

Instance Property

# preferredSplitBehavior

The preferred behavior that determines how the child view controllers appear in relation to each other.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var preferredSplitBehavior: UISplitViewController.SplitBehavior { get set }
```

## Discussion

Use this property to specify the split behavior that you prefer to use. The split view controller makes every effort to adopt the behavior you specify, but may use a different type of interface if there isn’t enough space to support your preferred choice. If changing the value of this property leads to an actual change in the current split behavior, the split view controller reflects the actual split behavior in the splitBehavior property. This change takes effect after the next layout occurs.

You do not set the split behavior directly; instead, you set a preferred split behavior by using the preferredSplitBehavior property. This change takes effect after the next layout occurs. The split view controller reflects the actual split behavior in the splitBehavior property. The value of the splitBehavior property affects which display modes are available for the split view controller. For possible configurations, see UISplitViewController.SplitBehavior.

Setting the value of this property to UISplitViewController.SplitBehavior.automatic causes the split view controller to choose the most appropriate display mode for the currently available space. The default value of this property is UISplitViewController.SplitBehavior.automatic.

## See Also

### Managing the split behavior

var splitBehavior: UISplitViewController.SplitBehavior

The current behavior that determines how the child view controllers appear in relation to each other.

enum SplitBehavior

Constants that describe the possible ways that the child view controllers appear in relation to each other.

