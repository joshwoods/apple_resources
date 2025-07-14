

- UIKit
-  UIScrollView 

Class

# UIScrollView

A view that allows the scrolling and zooming of its contained views.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIScrollView
```

## Overview

UIScrollView is the superclass of several UIKit classes, including UITableView and UITextView.

A scroll view is a view with an origin that’s adjustable over the content view. It clips the content to its frame, which generally (but not necessarily) coincides with that of the app’s main window. A scroll view tracks the movements of fingers, and adjusts the origin accordingly. The view that shows its content through the scroll view draws that portion of itself according to the new origin, which is pinned to an offset in the content view. The scroll view itself does no drawing except for displaying vertical and horizontal scroll indicators. The scroll view must know the size of the content view so it knows when to stop scrolling. By default, it *bounces* back when scrolling exceeds the bounds of the content.

The object that manages the drawing of content that displays in a scroll view needs to tile the content’s subviews so that no view exceeds the size of the screen. As users scroll in the scroll view, this object adds and removes subviews as necessary.

Because a scroll view has no scroll bars, it must know whether a touch signals an intent to scroll versus an intent to track a subview in the content. To make this determination, it temporarily intercepts a touch-down event by starting a timer and, before the timer fires, seeing if the touching finger makes any movement. If the timer fires without a significant change in position, the scroll view sends tracking events to the touched subview of the content view. If the user then drags their finger far enough before the timer elapses, the scroll view cancels any tracking in the subview and performs the scrolling itself. Subclasses can override the touchesShouldBegin(_:with:in:), isPagingEnabled, and touchesShouldCancel(in:) methods (which the scroll view calls) to affect how the scroll view handles scrolling gestures.

A scroll view also handles zooming and panning of content. As the user makes a pinch-in or pinch-out gesture, the scroll view adjusts the offset and the scale of the content. When the gesture ends, the object managing the content view updates subviews of the content as necessary. (Note that the gesture can end and a finger might still be down.) While the gesture is in progress, the scroll view doesn’t send any tracking calls to the subview.

The UIScrollView class can have a delegate that must adopt the UIScrollViewDelegate protocol. For zooming and panning to work, the delegate must implement both viewForZooming(in:) and scrollViewDidEndZooming(_:with:atScale:). In addition, the maximumZoomScale and minimumZoomScale zoom scales must be different.

### State preservation

If you assign a value to this view’s restorationIdentifier property, it attempts to preserve its scrolling-related information between app launches. Specifically, the values of the zoomScale, contentInset, and contentOffset properties are preserved. During restoration, the scroll view restores these values so that the content appears scrolled to the same position as before. For more information about how state preservation and restoration works, see App Programming Guide for iOS.

## Topics

### Responding to scroll view interactions

var delegate: (any UIScrollViewDelegate)?

The delegate of the scroll view.

protocol UIScrollViewDelegate

The interface for the delegate of a scroll view.

### Managing the content size and offset

var contentSize: CGSize

The size of the content view.

var contentOffset: CGPoint

The point at which the origin of the content view is offset from the origin of the scroll view.

func setContentOffset(CGPoint, animated: Bool)

Sets the offset from the content view’s origin that corresponds to the scroll view’s origin.

### Managing the content inset behavior

var adjustedContentInset: UIEdgeInsets

The insets derived from the content insets and the safe area of the scroll view.

var contentInset: UIEdgeInsets

The custom distance that the content view is inset from the safe area or scroll view edges.

var contentInsetAdjustmentBehavior: UIScrollView.ContentInsetAdjustmentBehavior

The behavior for determining the adjusted content offsets.

enum ContentInsetAdjustmentBehavior

Constants indicating how safe area insets are added to the adjusted content inset.

func adjustedContentInsetDidChange()

Notifies the scroll view when the adjusted content insets of the scroll view change.

### Getting the layout guides

var frameLayoutGuide: UILayoutGuide

The layout guide based on the untransformed frame rectangle of the scroll view.

var contentLayoutGuide: UILayoutGuide

The layout guide based on the untranslated content rectangle of the scroll view.

### Configuring the scroll view

var isScrollEnabled: Bool

A Boolean value that determines whether scrolling is enabled.

var isDirectionalLockEnabled: Bool

A Boolean value that determines whether scrolling is disabled in a particular direction.

var isPagingEnabled: Bool

A Boolean value that determines whether paging is enabled for the scroll view.

var scrollsToTop: Bool

A Boolean value that controls whether the scroll-to-top gesture is enabled.

var bounces: Bool

A Boolean value that controls whether the scroll view bounces past the edge of content and back again.

var bouncesHorizontally: Bool

A Boolean value that determines whether the scroll view bounces when it reaches the ends of its horizontal axis.

var bouncesVertically: Bool

A Boolean value that determines whether the scroll view bounces when it reaches the ends of its vertical axis.

var alwaysBounceVertical: Bool

A Boolean value that determines whether bouncing always occurs when vertical scrolling reaches the end of the content.

var alwaysBounceHorizontal: Bool

A Boolean value that determines whether bouncing always occurs when horizontal scrolling reaches the end of the content view.

### Managing the scrolling state

var isTracking: Bool

A Boolean value that indicates whether the user has touched the content to initiate scrolling.

var isDragging: Bool

A Boolean value that indicates whether the user has begun scrolling the content.

var isDecelerating: Bool

A Boolean value that indicates whether the content is moving in the scroll view after the user lifted their finger.

var isScrollAnimating: Bool

A Boolean value that indicates whether the scroll view is currently animating a scroll update.

func stopScrollingAndZooming()

Stops active scroll and zoom animations.

var decelerationRate: UIScrollView.DecelerationRate

A floating-point value that determines the rate of deceleration after the user lifts their finger.

struct DecelerationRate

Deceleration rates for the scroll view.

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

class UIRefreshControl

A standard control that can initiate the refreshing of a scroll view’s contents.

### Scrolling to a specific location

func scrollRectToVisible(CGRect, animated: Bool)

Scrolls a specific area of the content so that it’s visible in the scroll view.

### Managing touches

func touchesShouldBegin(Set&lt;UITouch>, with: UIEvent?, in: UIView) -> Bool

Overridden by subclasses to customize the default behavior when a finger touches down in displayed content.

func touchesShouldCancel(in: UIView) -> Bool

Returns whether to cancel touches related to the content subview and start dragging.

var canCancelContentTouches: Bool

A Boolean value that controls whether touches in the content view always lead to tracking.

var delaysContentTouches: Bool

A Boolean value that determines whether the scroll view delays the handling of touch-down gestures.

var directionalPressGestureRecognizer: UIGestureRecognizer

The underlying gesture recognizer for directional button presses.

### Zooming and panning

var panGestureRecognizer: UIPanGestureRecognizer

The underlying gesture recognizer for pan gestures.

var pinchGestureRecognizer: UIPinchGestureRecognizer?

The underlying gesture recognizer for pinch gestures.

func zoom(to: CGRect, animated: Bool)

Zooms to a specific area of the content so that it’s visible in the scroll view.

var zoomScale: CGFloat

A floating-point value that specifies the current scale factor applied to the scroll view’s content.

func setZoomScale(CGFloat, animated: Bool)

A floating-point value that specifies the current zoom scale.

var maximumZoomScale: CGFloat

A floating-point value that specifies the maximum scale factor that can apply to the scroll view’s content.

var minimumZoomScale: CGFloat

A floating-point value that specifies the minimum scale factor that can apply to the scroll view’s content.

var isZoomBouncing: Bool

A Boolean value that indicates that zooming has exceeded the scaling limits specified for the scroll view.

var isZooming: Bool

A Boolean value that indicates whether the content view is currently zooming in or out.

var isZoomAnimating: Bool

A Boolean value that indicates whether the scroll view is currently animating a zoom update.

var bouncesZoom: Bool

A Boolean value that determines whether the scroll view animates the content scaling when the scaling exceeds the maximum or minimum limits.

### Dismissing the keyboard

var keyboardDismissMode: UIScrollView.KeyboardDismissMode

The manner in which the system dismisses the keyboard when a drag begins in the scroll view.

enum KeyboardDismissMode

Constants that determine how the system dismisses the keyboard when a drag begins in the scroll view.

### Managing the index

var indexDisplayMode: UIScrollView.IndexDisplayMode

The manner in which the index appears while the user is scrolling.

enum IndexDisplayMode

Defines constants that represent how the index appears while the user is scrolling.

### Controlling content alignment

var contentAlignmentPoint: CGPoint

A point where the scroll view anchors content that’s smaller than the scroll view’s frame.

### Nesting scroll views

var transfersHorizontalScrollingToParent: Bool

A Boolean value that determines whether the scroll view passes horizontal scroll events to a superview.

var transfersVerticalScrollingToParent: Bool

A Boolean value that determines whether the scroll view passes vertical scroll events to a superview.

### Deprecated

var scrollIndicatorInsets: UIEdgeInsets

The distance the scroll indicators are inset from the edge of the scroll view.

Deprecated

### Instance Properties

var allowsKeyboardScrolling: Bool

A Boolean value that determines whether the scroll view allows scrolling its content with hardware keyboard input.

## Relationships

### Inherits From

- UIView

### Inherited By

- UICollectionView
- UITableView
- UITextView

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
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UIFocusItemScrollableContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Container views

Autosizing Views for Localization in iOS

Add auto layout constraints to your app to achieve localizable views.

Collection views

Display nested views using a configurable and highly customizable layout.

Table views

Display data in a single column of customizable rows.

class UIStackView

A streamlined interface for laying out a collection of views in either a column or a row.

