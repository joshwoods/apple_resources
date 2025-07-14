

- UIKit
- UIViewController
-  collapseSecondaryViewController(\_:for:) 

Instance Method

# collapseSecondaryViewController(\_:for:)

Called when a split view controller transitions to a compact-width size class.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func collapseSecondaryViewController(
    _ secondaryViewController: UIViewController,
    for splitViewController: UISplitViewController
)
```

## Parameters 

`secondaryViewController`  

The secondary view controller associated with the split view controller.

`splitViewController`  

The current split view controller.

## Discussion

This method provides default behavior when you do not overwrite the splitViewController(_:collapseSecondary:onto:) method. The primary view controller associated with the split view controller is displayed.

## See Also

### Adapting to environment changes

func separateSecondaryViewController(for: UISplitViewController) -> UIViewController?

Called when a split view controller transitions to a regular-width size class.

