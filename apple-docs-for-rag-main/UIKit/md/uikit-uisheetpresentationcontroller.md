

- UIKit
-  UISheetPresentationController 

Class

# UISheetPresentationController

A presentation controller that manages the appearance and behavior of a sheet.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
class UISheetPresentationController
```

## Overview

UISheetPresentationController lets you present your view controller as a sheet. Before you present your view controller, configure the sheet presentation controller in its sheetPresentationController property with the behavior and appearance you want for your sheet.

```
// In a subclass of UIViewController, customize and present the sheet.
func showMyViewControllerInACustomizedSheet() {
    let viewControllerToPresent = MyViewController()
    if let sheet = viewControllerToPresent.sheetPresentationController {
        sheet.detents = [.medium(), .large()]
        sheet.largestUndimmedDetentIdentifier = .medium
        sheet.prefersScrollingExpandsWhenScrolledToEdge = false
        sheet.prefersEdgeAttachedInCompactHeight = true
        sheet.widthFollowsPreferredContentSizeWhenEdgeAttached = true
    }
    present(viewControllerToPresent, animated: true, completion: nil)
}
```

Sheet presentation controllers specify a sheet’s size based on a *detent*, a height where a sheet naturally rests. Detents allow a sheet to resize from one edge of its fully expanded frame while the other three edges remain fixed. You specify the detents that a sheet supports using detents, and monitor its most recently selected detent using selectedDetentIdentifier.

Related Sessions from WWDC21

Session 10063: Customize and Resize Sheets in UIKit

Session 10068: What’s new in UIKit

## Topics

### Specifying the height

var detents: [UISheetPresentationController.Detent]

The array of heights where a sheet can rest.

var selectedDetentIdentifier: UISheetPresentationController.Detent.Identifier?

The identifier of the most recently selected detent.

class Detent

An object that represents a height where a sheet naturally rests.

### Managing the delegate

var delegate: (any UISheetPresentationControllerDelegate)?

The delegate of the sheet presentation controller.

protocol UISheetPresentationControllerDelegate

The interface that an object implements to respond to size changes in a sheet presentation controller.

### Managing user interaction

var largestUndimmedDetentIdentifier: UISheetPresentationController.Detent.Identifier?

The largest detent that doesn’t dim the view underneath the sheet.

var prefersScrollingExpandsWhenScrolledToEdge: Bool

A Boolean value that determines whether scrolling expands the sheet to a larger detent.

### Managing the appearance

var prefersGrabberVisible: Bool

A Boolean value that determines whether the sheet shows a grabber at the top.

var prefersPageSizing: Bool

A Boolean value that indicates whether the sheet sizes itself for readable content.

var prefersEdgeAttachedInCompactHeight: Bool

A Boolean value that determines whether the sheet attaches to the bottom edge of the screen in a compact-height size class.

var widthFollowsPreferredContentSizeWhenEdgeAttached: Bool

A Boolean value that determines whether the sheet’s width matches its view controller’s preferred content size.

var preferredCornerRadius: CGFloat?

The corner radius that the sheet attempts to present with.

### Customizing the position

var sourceView: UIView?

The view that the sheet centers itself over.

### Working with custom detents

func invalidateDetents()

Notifies the sheet to re-evaluate its detent value in the next layout pass.

### Animating changes to the sheet

func animateChanges(() -> Void)

Animates the UI changes to the sheet’s properties.

## Relationships

### Inherits From

- UIPresentationController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UITraitChangeObservable
- UITraitEnvironment

## See Also

### Presentation management

Disabling the pull-down gesture for a sheet

Ensure a positive user experience when presenting a view controller as a sheet.

class UIPresentationController

An object that manages the transition animations and the presentation of view controllers onscreen.

