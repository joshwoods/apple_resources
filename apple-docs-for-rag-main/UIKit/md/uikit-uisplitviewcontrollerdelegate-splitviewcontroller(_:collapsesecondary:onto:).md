

- UIKit
- UISplitViewControllerDelegate
-  splitViewController(\_:collapseSecondary:onto:) 

Instance Method

# splitViewController(\_:collapseSecondary:onto:)

Asks the delegate to adjust the primary view controller and to incorporate the secondary view controller into the collapsed interface.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func splitViewController(
    _ splitViewController: UISplitViewController,
    collapseSecondary secondaryViewController: UIViewController,
    onto primaryViewController: UIViewController
) -> Bool
```

## Parameters 

`splitViewController`  

The split view controller whose interface is collapsing.

`secondaryViewController`  

The secondary view controller of the split view interface.

`primaryViewController`  

The primary view controller of the split view interface. If you implement the primaryViewController(forCollapsing:) method in your delegate, this object is the one that method returns.

## Return Value

false to let the split view controller try to incorporate the secondary view controller’s content into the collapsed interface, or true to indicate that you do not want the split view controller to do anything with the secondary view controller.

## Discussion

This delegate method only applies to classic split view interfaces. For more information, see Split view styles.

This method is your opportunity to perform any necessary tasks related to the transition to a collapsed interface. After this method returns, the split view controller removes the secondary view controller from its viewControllers array, leaving the primary view controller as its only child. In your implementation of this method, you might prepare the primary view controller for display in a compact environment, or you might attempt to incorporate the secondary view controller’s content into the newly collapsed interface.

Returning false tells the split view controller to use its default behavior to try to incorporate the secondary view controller into the collapsed interface. When you return false, the split view controller calls the collapseSecondaryViewController(_:for:) method of the primary view controller, giving it a chance to do something with the secondary view controller’s content. Most view controllers do nothing by default, but the UINavigationController class responds by pushing the secondary view controller onto its navigation stack.

Returning true from this method tells the split view controller not to apply any default behavior. You might return true in cases where you do not want the secondary view controller’s content incorporated into the resulting interface.

## See Also

### Collapsing and expanding classic split views

func primaryViewController(forCollapsing: UISplitViewController) -> UIViewController?

Asks the delegate to provide the single view controller to display after the split view interface collapses.

func primaryViewController(forExpanding: UISplitViewController) -> UIViewController?

Asks the delegate to provide the view controller to display in the primary position when the split view interface expands.

func splitViewController(UISplitViewController, separateSecondaryFrom: UIViewController) -> UIViewController?

Asks the delegate to provide the new secondary view controller for the split view interface.

