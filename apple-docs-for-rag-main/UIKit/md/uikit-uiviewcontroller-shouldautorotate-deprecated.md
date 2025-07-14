

- UIKit
- UIViewController
-  shouldAutorotate Deprecated

Instance Property

# shouldAutorotate

A Boolean value that indicates whether the view controller’s contents should autorotate.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var shouldAutorotate: Bool { get }
```

Deprecated

Instead, update supportedInterfaceOrientations and then call setNeedsUpdateOfSupportedInterfaceOrientations() to indicate a change to the supported interface orientations.

## Return Value

true if the content should rotate, otherwise false. This method returns true by default.

## See Also

### Deprecated properties

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

var searchDisplayController: UISearchDisplayController?

The search display controller associated with the view controller.

Deprecated

var topLayoutGuide: any UILayoutSupport

Indicates the highest vertical extent for your onscreen content, for use with Auto Layout constraints.

Deprecated

