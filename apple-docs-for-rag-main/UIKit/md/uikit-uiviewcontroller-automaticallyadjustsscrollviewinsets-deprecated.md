

- UIKit
- UIViewController
-  automaticallyAdjustsScrollViewInsets Deprecated

Instance Property

# automaticallyAdjustsScrollViewInsets

A Boolean value that indicates whether the view controller should automatically adjust its scroll view insets.

iOS 7.0–11.0DeprecatediPadOS 7.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 7.0–11.0Deprecated

``` source
@MainActor
var automaticallyAdjustsScrollViewInsets: Bool { get set }
```

## Discussion

The default value of this property is true, which lets container view controllers know that they should adjust the scroll view insets of this view controller’s view to account for screen areas consumed by a status bar, search bar, navigation bar, toolbar, or tab bar. Set this property to false if your view controller implementation manages its own scroll view inset adjustments.

## See Also

### Deprecated properties

var shouldAutorotate: Bool

A Boolean value that indicates whether the view controller’s contents should autorotate.

Deprecated

var previewActionItems: [any UIPreviewActionItem]

The quick actions displayed when a user swipes upward on a 3D Touch preview.

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

