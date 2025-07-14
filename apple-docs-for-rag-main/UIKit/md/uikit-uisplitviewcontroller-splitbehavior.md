

- UIKit
- UISplitViewController
-  splitBehavior 

Instance Property

# splitBehavior

The current behavior that determines how the child view controllers appear in relation to each other.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var splitBehavior: UISplitViewController.SplitBehavior { get }
```

## Discussion

This property controls how a split view controller’s secondary view controller appears in relation to the other child view controllers. To change the current split behavior, change the value of the preferredSplitBehavior property.

The value of this property affects which display modes are available for the split view interface. For possible configurations, see UISplitViewController.SplitBehavior.

## See Also

### Managing the split behavior

var preferredSplitBehavior: UISplitViewController.SplitBehavior

The preferred behavior that determines how the child view controllers appear in relation to each other.

enum SplitBehavior

Constants that describe the possible ways that the child view controllers appear in relation to each other.

