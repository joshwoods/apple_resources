

- UIKit
-  UIViewControllerRestoration 

Protocol

# UIViewControllerRestoration

The methods that objects adopt so that they can act as a restoration class for view controllers during state restoration.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIViewControllerRestoration
```

## Overview

To use a class that adopts this protocol, you must assign that class to the restorationClass property of one of your app’s view controllers. The method in this protocol should be used to create the view controller, if it doesn’t yet exist, or return an existing view controller object, if one does exist.

## Topics

### Creating the view controller

static func viewController(withRestorationIdentifierPath: [String], coder: NSCoder) -> UIViewController?

Requests the view controller that corresponds to the specified identifier information.

**Required**

## See Also

### Interface restoration

Restoring your app’s state

Provide continuity for the user by preserving current activities.

Restoring Your App’s State with SwiftUI

Provide app continuity for users by preserving their current activities.

Preserving your app’s UI across launches

Return your app to its previous state after the system terminates it.

protocol UIObjectRestoration

The interface that restoration classes use to restore preserved objects.

protocol UIStateRestoring

Methods for adding objects to your state restoration archives.

