

- UIKit
-  UIStateRestoring 

Protocol

# UIStateRestoring

Methods for adding objects to your state restoration archives.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIStateRestoring : NSObjectProtocol
```

## Mentioned in 

About the UI preservation process

## Overview

You can add state restoring objects to an archive directly or by referencing them from another object that’s preserved, such as a view controller. The methods of the protocol let you save enough information about the object to find or recreate it during the next launch cycle.

When adopting this protocol in your custom objects, you must also remember to register those objects using the registerObject(forStateRestoration:restorationIdentifier:) method of the UIApplication class. You don’t need to register views or view controllers explicitly because UIKit registers those objects automatically. View controllers adopt this protocol so that they may be used as the restoration parent of one of your custom objects.

## Topics

### Accessing the object information

var restorationParent: (any UIStateRestoring)?

The parent object used to scope the current object.

var objectRestorationClass: (any UIObjectRestoration.Type)?

The class responsible for creating this object when restoring the app’s state.

### Encoding and decoding the object

func encodeRestorableState(with: NSCoder)

Encodes state-related information for the object.

func decodeRestorableState(with: NSCoder)

Decodes and restores state-related information for the object.

func applicationFinishedRestoringState()

Called after all objects have had a chance to decode their state.

### Constants

State restoration keys

Keys that are available in restoration archives.

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
- UIReferenceLibraryViewController
- UISearchContainerViewController
- UISearchController
- UISplitViewController
- UITabBarController
- UITableViewController
- UITextFormattingViewController
- UIVideoEditorController
- UIViewController

## See Also

### Interface restoration

Restoring your app’s state

Provide continuity for the user by preserving current activities.

Restoring Your App’s State with SwiftUI

Provide app continuity for users by preserving their current activities.

Preserving your app’s UI across launches

Return your app to its previous state after the system terminates it.

protocol UIViewControllerRestoration

The methods that objects adopt so that they can act as a restoration class for view controllers during state restoration.

protocol UIObjectRestoration

The interface that restoration classes use to restore preserved objects.

