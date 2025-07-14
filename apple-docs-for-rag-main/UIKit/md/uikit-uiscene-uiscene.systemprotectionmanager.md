

- UIKit
- UIScene
-  UIScene.SystemProtectionManager 

Class

# UIScene.SystemProtectionManager

A class that represents the status of system protection for the scene.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor
class SystemProtectionManager
```

## Overview

Use this class to determine if the system protects a scene, such as by locking the app and requiring authentication with Face ID or Touch ID. You may want to disable your own app’s privacy shielding if the system already requires authentication.

The following example shows how a scene can use the manager’s isUserAuthenticationEnabled property to decide whether to provide its own UI shielding. When the scene becomes active, the app shows an authentication challenge if the system doesn’t already provide protection. When the scene resigns the active role, the app provides its own shielding only if the system isn’t already doing so.

- Swift
- Objective-C

```
func sceneDidBecomeActive(_ scene: UIScene) {
    guard scene.systemProtectionManager?.isUserAuthenticationEnabled ?? false else {
        // Show custom authentication.
    }
}

func sceneWillResignActive(_ scene: UIScene) {
    guard scene.systemProtectionManager?.isUserAuthenticationEnabled ?? false else {
        // Show custom shield to hide sensitive information.
    }
}

```

```
- (void)sceneDidBecomeActive:(UIScene *)scene {
    if ( scene.systemProtectionManager.userAuthenticationEnabled ) {
        // Don't show custom authentication.
    } else {
        // Show custom shield to hide sensitive information.
    }
}

- (void)sceneWillResignActive:(UIScene *)scene {
    if ( scene.systemProtectionManager.userAuthenticationEnabled ) {
        // Don't show custom shield; system already does so.
    } else {
        // Show custom shield to hide sensitive information.
    }
}
```

## Topics

### Inspecting protection state

var isUserAuthenticationEnabled: Bool

The current status of system user authentication.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Working with system protection manager

var systemProtectionManager: UIScene.SystemProtectionManager?

The system protection manager associated with this scene.

class let systemProtectionDidChangeNotification: NSNotification.Name

A notification posted when the system-protection attributes of a scene change.

