

- UIKit
- Touches, presses, and gestures
- Tracking the force of 3D Touch events
-  Checking the availability of 3D Touch 

Article

# Checking the availability of 3D Touch

Check whether a device supports 3D Touch before enabling features that use it.

## Overview

To determine if 3D Touch is available on a device, check the forceTouchCapability property of any object — such as your app’s views and view controllers — that adopts the UITraitEnvironment protocol. The following code shows how you might use this property to enable or disable features at load time from your view controller. Use the traitCollectionDidChange(_:) method to detect changes to 3D Touch availability while your app is running.

```
class ViewController: UIViewController {
    override func viewDidLoad() {
        super.viewDidLoad()

        // Check the trait collection to see if force is available.
        if self.traitCollection.forceTouchCapability == .available {
            // Enable 3D Touch features
        } else {
            // Fall back to other non 3D Touch features.
        }
    }

    override func traitCollectionDidChange(_ previousTraitCollection: UITraitCollection?) {
        // Update the app's 3D Touch support.
        if self.traitCollection.forceTouchCapability == .available {
            // Enable 3D Touch features
        } else {
            // Fall back to other non 3D Touch features.
        }
    }
}
```

For guidance on how to implement your app both with and without 3D Touch support, see iOS Human Interface Guidelines.

