

- UIKit
-  UICoordinateSpace 

Protocol

# UICoordinateSpace

A set of methods for converting between different frames of reference on a screen.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UICoordinateSpace : NSObjectProtocol
```

## Overview

The UIView class adopts this protocol so that you can convert easily between most coordinate spaces in your app. The UIScreen class includes the coordinateSpace and fixedCoordinateSpace properties, which give you access to the screen’s coordinate spaces. You can adopt this protocol in your own classes to convert between your custom coordinate spaces and the coordinate spaces of your app’s views and screens.

In iOS 8 and later, window and screen coordinate spaces aren’t fixed to a specific device orientation. Instead, window and screen coordinates change to match the app’s interface orientation, which typically (but not always) matches the current device orientation. (View controllers still determine which interface orientations the app supports.) Rotating the window and screen simplifies the interactions between views, windows, and the screen. In cases where you still need a fixed frame of reference — for example, because you need to store the location of a touch event or onscreen item persistently — you can use the methods of this protocol to convert coordinate values to the fixed coordinate space provided by the UIScreen object.

To convert a point from a view’s current coordinate space to the screen’s fixed coordinate space, use code similar to the following:

```
[myView convertPoint:point toCoordinateSpace:myView.window.screen.fixedCoordinateSpace];
```

When implementing the methods of this protocol, you must convert coordinate values to or from your local coordinate space. When performing such conversions, use the screen coordinate space as an intermediate coordinate space, converting to screen coordinates before converting to the target coordinate space. For example, when converting from your local coordinate space to the coordinate space of another view, convert your local coordinates to the screen coordinate space first and then convert those screen coordinates to the coordinate space of the view.

## Topics

### Getting the bounds rectangle

var bounds: CGRect

The bounds rectangle describing the item’s location and size in its own coordinate system.

**Required**

### Converting between coordinate spaces

func convert(CGPoint, to: any UICoordinateSpace) -> CGPoint

Converts a point from the coordinate space of the current object to the specified coordinate space.

**Required**

func convert(CGPoint, from: any UICoordinateSpace) -> CGPoint

Converts a point from the specified coordinate space to the coordinate space of the current object.

**Required**

func convert(CGRect, to: any UICoordinateSpace) -> CGRect

Converts a rectangle from the coordinate space of the current object to the specified coordinate space.

**Required**

func convert(CGRect, from: any UICoordinateSpace) -> CGRect

Converts a rectangle from the specified coordinate space to the coordinate space of the current object.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- UITextCursorView
- UITextSelectionHandleView
- UITextSelectionHighlightView

### Conforming Types

- UIActionSheet
- UIActivityIndicatorView
- UIAlertView
- UIButton
- UICalendarView
- UICollectionReusableView
- UICollectionView
- UICollectionViewCell
- UICollectionViewListCell
- UIColorWell
- UIContentUnavailableView
- UIControl
- UIDatePicker
- UIEventAttributionView
- UIImageView
- UIInputView
- UILabel
- UIListContentView
- UINavigationBar
- UIPageControl
- UIPasteControl
- UIPickerView
- UIPopoverBackgroundView
- UIProgressView
- UIRefreshControl
- UIScrollView
- UISearchBar
- UISearchTextField
- UISegmentedControl
- UISlider
- UIStackView
- UIStandardTextCursorView
- UIStepper
- UISwitch
- UITabBar
- UITableView
- UITableViewCell
- UITableViewHeaderFooterView
- UITextField
- UITextView
- UIToolbar
- UIView
- UIVisualEffectView
- UIWebView
- UIWindow

## See Also

### Windows

class UIWindow

The backdrop for your app’s user interface and the object that dispatches events to your views.

