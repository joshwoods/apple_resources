

- UIKit
-  UIViewControllerPreviewing Deprecated

Protocol

# UIViewControllerPreviewing

A set of methods that define the interface for configuring a previewing view controller on devices that support 3D Touch.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIViewControllerPreviewing : NSObjectProtocol
```

Deprecated

Use UIContextMenuInteraction instead.

## Overview

The system returns a context object conforming to this protocol when you call a view controller’s registerForPreviewing(with:sourceView:) method. This method registers the view controller to participate in 3D Touch preview (peek) and commit (pop) behaviors.

Terminology Note

The end-user terminology for the views presented during the phases of force-based touches includes *peek* and *pop*. For clarity here, and to align with the API names, this document uses the corresponding terms *preview* and *commit view*.

To learn about 3D Touch, read Adopting 3D Touch on iPhone.

Important

Don’t adopt this protocol in custom classes.

## Topics

### Configuring a source view for a 3D Touch previewing view controller

var sourceRect: CGRect

The rectangle, in the source view’s coordinate system, that responds to a 3D Touch by a user and remains visually sharp while surrounding content blurs.

**Required**

var previewingGestureRecognizerForFailureRelationship: UIGestureRecognizer

A gesture recognizer suitable for setting up failure requirements for a preview’s (peek’s) gestures.

**Required**

### Accessing properties of a 3D Touch previewing view controller

var delegate: any UIViewControllerPreviewingDelegate

The previewing view controller’s delegate for managing preview (peek) and commit (pop) view controllers.

**Required**

var sourceView: UIView

A source view, in a previewing view controller’s view hierarchy, responds to a 3D Touch by the user.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Deprecated protocols

protocol UIAccelerometerDelegate

The interface for receiving acceleration-related data from the system.

Deprecated

protocol UIActionSheetDelegate

The interface for the delegate of an action sheet object.

Deprecated

protocol UIAlertViewDelegate

The interface for the delegate of an alert view object.

Deprecated

protocol UIPopoverControllerDelegate

The interface for the delegate of a popover controller object.

Deprecated

protocol UISearchDisplayDelegate

The interface for the delegate of a search display controller.

Deprecated

protocol UIViewControllerPreviewingDelegate

A set of methods used by the delegate to respond, with a preview view controller and a commit view controller, to the user pressing a view object on the screen of a device that supports 3D Touch.

Deprecated

