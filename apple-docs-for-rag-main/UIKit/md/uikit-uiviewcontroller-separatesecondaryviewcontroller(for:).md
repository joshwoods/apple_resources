

- UIKit
- UIViewController
-  separateSecondaryViewController(for:) 

Instance Method

# separateSecondaryViewController(for:)

Called when a split view controller transitions to a regular-width size class.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func separateSecondaryViewController(for splitViewController: UISplitViewController) -> UIViewController?
```

## Parameters 

`splitViewController`  

The current split view controller.

## Return Value

The designated secondary view controller for the split view controller.

## Discussion

This method provides default behavior when you do not overwrite the splitViewController(_:separateSecondaryFrom:) method. The previous secondary view controller is returned.

## See Also

### Adapting to environment changes

func collapseSecondaryViewController(UIViewController, for: UISplitViewController)

Called when a split view controller transitions to a compact-width size class.

