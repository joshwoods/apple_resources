

- UIKit
- UIViewController
-  searchDisplayController Deprecated

Instance Property

# searchDisplayController

The search display controller associated with the view controller.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
var searchDisplayController: UISearchDisplayController? { get }
```

Deprecated

Use the UISearchController class to integrate search results.

## Discussion

This property reflects the value of the `searchDisplayController` outlet that you set in Interface Builder. If you create your search display controller programmatically, this property is set automatically by the search display controller when it is initialized.

## See Also

### Deprecated properties

var shouldAutorotate: Bool

A Boolean value that indicates whether the view controller’s contents should autorotate.

Deprecated

var previewActionItems: [any UIPreviewActionItem]

The quick actions displayed when a user swipes upward on a 3D Touch preview.

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

var topLayoutGuide: any UILayoutSupport

Indicates the highest vertical extent for your onscreen content, for use with Auto Layout constraints.

Deprecated

