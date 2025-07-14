

- UIKit
-  UIRefreshControl 

Class

# UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIRefreshControl
```

## Mentioned in 

Choosing a user interface idiom for your Mac app

## Overview

A UIRefreshControl object is a standard control that you attach to any UIScrollView object, including table views and collection views. Add this control to scrollable views to give your users a standard way to refresh their contents. When the user drags the top of the scrollable content area downward, the scroll view reveals the refresh control, begins animating its progress indicator, and notifies your app. You use that notification to update your content and dismiss the refresh control.

The refresh control lets you know when to update your content using the target-action mechanism of UIControl. Upon activation, the refresh control calls the action method you provided at configuration time. When adding your action method, configure it to listen for the valueChanged event, as shown in the following example code. Use your action method to update your content, and call the refresh control’s endRefreshing() method when you’re done.

```
func configureRefreshControl () {
   // Add the refresh control to your UIScrollView object.
   myScrollingView.refreshControl = UIRefreshControl()
   myScrollingView.refreshControl?.addTarget(self, action:
                                      #selector(handleRefreshControl),
                                      for: .valueChanged)
}

@objc func handleRefreshControl() {
   // Update your content…

   // Dismiss the refresh control.
   DispatchQueue.main.async {
      self.myScrollingView.refreshControl?.endRefreshing()
   }
}

```

If you’re using a UITableViewController, assign its refreshControl property to an instance of UIRefreshControl. Then associate a target and action method for the valueChanged event to manage the refresh behavior of the associated table view.

Important

UIRefreshControl isn’t available when the user interface idiom is UIUserInterfaceIdiom.mac. However, you can update your app to provide similar functionality in the Mac idiom. For example, replace the control with a Refresh menu item by creating a UIKeyCommand object with the title “Refresh” and the keyboard shortcut Command-R. Then add the command to your app’s menu system. For more information, see Adding menus and shortcuts to the menu bar and user interface.

## Topics

### Initializing a refresh control

init()

Initializes and returns a standard refresh control.

### Accessing the control attributes

var tintColor: UIColor!

The tint color for the refresh control.

var attributedTitle: NSAttributedString?

The styled title text to display in the refresh control.

### Managing the refresh status

func beginRefreshing()

Tells the control that a refresh operation was started programmatically.

func endRefreshing()

Tells the control that a refresh operation has ended.

var isRefreshing: Bool

A Boolean value indicating whether a refresh operation has been triggered and is in progress.

## Relationships

### Inherits From

- UIControl

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UIContextMenuInteractionDelegate
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Managing the scroll indicator and refresh control

var indicatorStyle: UIScrollView.IndicatorStyle

The style of the scroll indicators.

enum IndicatorStyle

Defines constants that represent the styles of the scroll indicators.

var showsHorizontalScrollIndicator: Bool

A Boolean value that controls whether the horizontal scroll indicator is visible.

var showsVerticalScrollIndicator: Bool

A Boolean value that controls whether the vertical scroll indicator is visible.

var horizontalScrollIndicatorInsets: UIEdgeInsets

The horizontal distance the scroll indicators are inset from the edge of the scroll view.

var verticalScrollIndicatorInsets: UIEdgeInsets

The vertical distance the scroll indicators are inset from the edge of the scroll view.

var automaticallyAdjustsScrollIndicatorInsets: Bool

A Boolean value that indicates whether the system automatically adjusts the scroll indicator insets.

func flashScrollIndicators()

Displays the scroll indicators momentarily.

func withScrollIndicatorsShown(forContentOffsetChanges: () -> Void)

Displays the scroll indicators during updates to the scroll view’s content offset.

var refreshControl: UIRefreshControl?

The refresh control associated with the scroll view.

