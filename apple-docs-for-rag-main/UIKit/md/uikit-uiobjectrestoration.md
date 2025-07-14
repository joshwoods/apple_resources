

- UIKit
-  UIObjectRestoration 

Protocol

# UIObjectRestoration

The interface that restoration classes use to restore preserved objects.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIObjectRestoration
```

## Overview

A restorable object must set its objectRestorationClass property to the class that adopts this protocol. The method in this protocol should be used to return the object if it already exists or create it if needed.

## Topics

### Creating the restorable object

static func object(withRestorationIdentifierPath: [String], coder: NSCoder) -> (any UIStateRestoring)?

Requests the object that corresponds to the specified identifier information.

**Required**

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

protocol UIStateRestoring

Methods for adding objects to your state restoration archives.

