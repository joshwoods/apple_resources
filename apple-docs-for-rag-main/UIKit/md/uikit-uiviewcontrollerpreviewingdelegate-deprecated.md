

- UIKit
-  UIViewControllerPreviewingDelegate Deprecated

Protocol

# UIViewControllerPreviewingDelegate

A set of methods used by the delegate to respond, with a preview view controller and a commit view controller, to the user pressing a view object on the screen of a device that supports 3D Touch.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
protocol UIViewControllerPreviewingDelegate : NSObjectProtocol
```

Deprecated

Use UIContextMenuInteractionDelegate instead.

## Overview

To learn about 3D Touch, read Adopting 3D Touch on iPhone.

Terminology Note

The end-user terminology for the views presented during the phases of force-based touches includes *peek* and *pop*. For clarity here, and to align with the API names, this document uses the corresponding terms *preview* and *commit view*.

## Topics

### Providing preview and commit views for 3D Touch

func previewingContext(any UIViewControllerPreviewing, viewControllerForLocation: CGPoint) -> UIViewController?

Called when the user has pressed a source view in a previewing view controller, thereby obtaining a surrounding blur to indicate that a preview (peek) is available.

**Required**

func previewingContext(any UIViewControllerPreviewing, commit: UIViewController)

Called to let you prepare the presentation of a commit (pop) view from your commit view controller.

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

protocol UIViewControllerPreviewing

A set of methods that define the interface for configuring a previewing view controller on devices that support 3D Touch.

Deprecated

