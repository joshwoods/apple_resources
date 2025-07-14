

- UIKit
- UISplitViewControllerDelegate
-  primaryViewController(forExpanding:) 

Instance Method

# primaryViewController(forExpanding:)

Asks the delegate to provide the view controller to display in the primary position when the split view interface expands.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func primaryViewController(forExpanding splitViewController: UISplitViewController) -> UIViewController?
```

## Parameters 

`splitViewController`  

The split view controller whose interface is expanding.

## Return Value

The view controller to use as the primary view controller, or `nil` to specify the current primary view controller.

## Discussion

This delegate method only applies to classic split view interfaces. For more information, see Split view styles.

When the split view controller transitions from a horizontally compact to a horizontally regular size class, it calls this method and asks you for the view controller to display in the primary position when that transition is complete. The view controller you return becomes the primary view controller of the split view interface. If you do not implement this method, or if your implementation returns `nil`, the split view controller chooses its current primary view controller as the one to use.

If you specified a specific view controller in your primaryViewController(forCollapsing:) method, use this method to restore the original primary view controller for your split view interface. You can also implement the splitViewController(_:separateSecondaryFrom:) method to disentangle your view controllers from one another as needed.

## See Also

### Collapsing and expanding classic split views

func primaryViewController(forCollapsing: UISplitViewController) -> UIViewController?

Asks the delegate to provide the single view controller to display after the split view interface collapses.

func splitViewController(UISplitViewController, collapseSecondary: UIViewController, onto: UIViewController) -> Bool

Asks the delegate to adjust the primary view controller and to incorporate the secondary view controller into the collapsed interface.

func splitViewController(UISplitViewController, separateSecondaryFrom: UIViewController) -> UIViewController?

Asks the delegate to provide the new secondary view controller for the split view interface.

