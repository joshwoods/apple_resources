

- UIKit
- UIViewController
-  previewActionItems Deprecated

Instance Property

# previewActionItems

The quick actions displayed when a user swipes upward on a 3D Touch preview.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
var previewActionItems: [any UIPreviewActionItem] { get }
```

Deprecated

Use UIContextMenuInteraction instead.

## Return Value

An array of preview (peek) quick actions.

## Discussion

This property is for use with a preview (peek) view controller which you present in your implementation of the previewingContext(_:viewControllerForLocation:) delegate method..

Implement this method to provide quick actions for such a preview. When the user swipes upward on the preview, the system presents these quick action items in a sheet below the preview.

The default implementation of this method returns an empty array.

For guidance on appropriate items to include as preview quick actions, read the material on 3D Touch in the iOS Technologies chapter of iOS Human Interface Guidelines.

For more information on preview quick actions, see UIPreviewActionItem and UIPreviewAction.

## See Also

### Deprecated properties

var shouldAutorotate: Bool

A Boolean value that indicates whether the view controller’s contents should autorotate.

Deprecated

var automaticallyAdjustsScrollViewInsets: Bool

A Boolean value that indicates whether the view controller should automatically adjust its scroll view insets.

Deprecated

var bottomLayoutGuide: any UILayoutSupport

Indicates the lowest vertical extent for your onscreen content, for use with Auto Layout constraints.

Deprecated

var interfaceOrientation: UIInterfaceOrientation

Convenience property that provides the current orientation of the interface, meaningful only if the view controller is taking up the full screen.

Deprecated

var isModalInPopover: Bool

A Boolean value indicating whether the view controller should be presented modally by a popover.

Deprecated

var searchDisplayController: UISearchDisplayController?

The search display controller associated with the view controller.

Deprecated

var topLayoutGuide: any UILayoutSupport

Indicates the highest vertical extent for your onscreen content, for use with Auto Layout constraints.

Deprecated

