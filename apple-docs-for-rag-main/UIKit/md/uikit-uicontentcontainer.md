

- UIKit
-  UIContentContainer 

Protocol

# UIContentContainer

A set of methods for adapting the contents of your view controllers to size and trait changes.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIContentContainer : NSObjectProtocol
```

## Overview

The methods of this protocol handle size-related transitions that are related to changes in the current trait environment or view controller hierarchy. When the parent view controller changes, or when trait changes occur that affect the size of a view controller, UIKit calls these methods to give the affected objects a chance to respond appropriately.

All UIViewController and UIPresentationController objects provide default implementations for the methods of this protocol. When creating your own custom view controller or presentation controller, you can override the default implementations to make adjustments to your content. For example, you might use these methods to adjust the size or position of any child view controllers.

When overriding the methods of this protocol, call `super` to let UIKit perform any default behaviors. View controllers and presentation controllers perform their own adjustments when these methods are called. Calling `super` ensures that UIKit is able to continue adjusting other parts of your user interface.

## Topics

### Responding to environment changes

func viewWillTransition(to: CGSize, with: any UIViewControllerTransitionCoordinator)

Notifies the container that the size of its view is about to change.

**Required**

func willTransition(to: UITraitCollection, with: any UIViewControllerTransitionCoordinator)

Notifies the container that its trait collection changed.

**Required**

### Responding to changes in child view controllers

func size(forChildContentContainer: any UIContentContainer, withParentContainerSize: CGSize) -> CGSize

Returns the size of the specified child view controller’s content.

**Required**

func preferredContentSizeDidChange(forChildContentContainer: any UIContentContainer)

Notifies an interested controller that the preferred content size of one of its children changed.

**Required**

func systemLayoutFittingSizeDidChange(forChildContentContainer: any UIContentContainer)

Notifies the container that a child view controller was resized using Auto Layout.

**Required**

var preferredContentSize: CGSize

The preferred size for the container’s content.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIActivityViewController
- UIAlertController
- UICloudSharingController
- UICollectionViewController
- UIColorPickerViewController
- UIDocumentBrowserViewController
- UIDocumentMenuViewController
- UIDocumentPickerExtensionViewController
- UIDocumentPickerViewController
- UIDocumentViewController
- UIFontPickerViewController
- UIImagePickerController
- UIInputViewController
- UINavigationController
- UIPageViewController
- UIPopoverPresentationController
- UIPresentationController
- UIReferenceLibraryViewController
- UISearchContainerViewController
- UISearchController
- UISheetPresentationController
- UISplitViewController
- UITabBarController
- UITableViewController
- UITextFormattingViewController
- UIVideoEditorController
- UIViewController

## See Also

### Adaptivity

Automatic trait tracking

Reduce the need to manually register for trait changes when you use traits within a method or closure that supports automatic trait tracking.

Responding to changing display modes on Apple TV

Change images and resources dynamically when the screen gamut on your device changes.

class UITraitCollection

A collection of data that represents the environment for an individual element in your app’s user interface.

protocol UITraitEnvironment

A set of methods that makes the iOS interface environment available to your app.

protocol UITraitChangeObservable

A type that calls your code in reaction to changes in the trait environment.

protocol UIMutableTraits

A mutable container of traits.

protocol UIAdaptivePresentationControllerDelegate

A set of methods that, in conjunction with a presentation controller, determine how to respond to trait changes in your app.

