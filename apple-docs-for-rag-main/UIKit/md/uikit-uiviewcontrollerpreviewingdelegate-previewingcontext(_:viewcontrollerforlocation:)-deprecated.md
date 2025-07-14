

- UIKit
- UIViewControllerPreviewingDelegate
-  previewingContext(\_:viewControllerForLocation:) Deprecated

Instance Method

# previewingContext(\_:viewControllerForLocation:)

Called when the user has pressed a source view in a previewing view controller, thereby obtaining a surrounding blur to indicate that a preview (peek) is available.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
func previewingContext(
    _ previewingContext: any UIViewControllerPreviewing,
    viewControllerForLocation location: CGPoint
) -> UIViewController?
```

**Required**

## Parameters 

`previewingContext`  

The context object for the previewing view controller.

`location`  

The location of the touch in the source view’s coordinate system.

## Return Value

The view controller whose view you want to provide as the preview (peek), or `nil` to disable preview..

## Discussion

Implement this method to return the preview view controller.

To indicate that a particular portion of the source view is responding to the user’s force touch, set the context object’s sourceRect property to the desired rectangle. For example, if the context object’s sourceView property is a table view, you can set the sourceRect property to the frame of the row indicated by the `location` parameter’s value. When the system presents the preview (peek), it appears to originate from the selected row.

You can disable preview by returning `nil` from this method.

## See Also

### Providing preview and commit views for 3D Touch

func previewingContext(any UIViewControllerPreviewing, commit: UIViewController)

Called to let you prepare the presentation of a commit (pop) view from your commit view controller.

**Required**

Deprecated

