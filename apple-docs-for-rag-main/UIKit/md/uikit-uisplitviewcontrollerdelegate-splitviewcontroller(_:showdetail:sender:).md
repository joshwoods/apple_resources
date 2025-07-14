

- UIKit
- UISplitViewControllerDelegate
-  splitViewController(\_:showDetail:sender:) 

Instance Method

# splitViewController(\_:showDetail:sender:)

Asks the delegate if it will do the work of displaying a view controller in the secondary position of the split view interface.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func splitViewController(
    _ splitViewController: UISplitViewController,
    showDetail vc: UIViewController,
    sender: Any?
) -> Bool
```

## Parameters 

`splitViewController`  

The split view controller whose secondary view controller is being updated.

`vc`  

The view controller being displayed in the secondary position.

`sender`  

The object that made the request.

## Return Value

true if you handled the presentation of the view controller, or false if you want the split view controller to do it.

## Discussion

This delegate method only applies to classic split view interfaces. For more information, see Split view styles.

When its showDetailViewController(_:sender:) method is called, the split view controller calls this method to see if your delegate will handle the presentation of the specified view controller. If you implement this method and ultimately return true, your implementation is responsible for presenting the specified view controller in the secondary position of the split view interface.

If you don’t implement this method or if your implementation returns false, the split view controller presents the view controller.

## See Also

### Overriding the presentation behavior

func splitViewController(UISplitViewController, show: UIViewController, sender: Any?) -> Bool

Asks the delegate if it will do the work of displaying a view controller in the primary position of the split view interface.

