

- UIKit
- UIViewControllerPreviewingDelegate
-  previewingContext(\_:commit:) Deprecated

Instance Method

# previewingContext(\_:commit:)

Called to let you prepare the presentation of a commit (pop) view from your commit view controller.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
func previewingContext(
    _ previewingContext: any UIViewControllerPreviewing,
    commit viewControllerToCommit: UIViewController
)
```

**Required**

## Parameters 

`previewingContext`  

The context object for the previewing view controller.

`viewControllerToCommit`  

The view controller whose view your implementation of this method is moving into place as a commit (pop) view.

## Discussion

Implement this method to configure and present the commit (pop) view controller, in a way that is appropriate for your app.

For example, to present the commit view controller’s view in a navigation controller, call the navigation controller’s show(_:sender:) method; to present the view modally, you could call the present(_:animated:completion:) method.

## See Also

### Providing preview and commit views for 3D Touch

func previewingContext(any UIViewControllerPreviewing, viewControllerForLocation: CGPoint) -> UIViewController?

Called when the user has pressed a source view in a previewing view controller, thereby obtaining a surrounding blur to indicate that a preview (peek) is available.

**Required**

Deprecated

