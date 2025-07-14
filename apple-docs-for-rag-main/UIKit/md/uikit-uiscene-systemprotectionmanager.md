

- UIKit
- UIScene
-  systemProtectionManager 

Instance Property

# systemProtectionManager

The system protection manager associated with this scene.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor
var systemProtectionManager: UIScene.SystemProtectionManager? { get }
```

## Discussion

To check whether the scene requires user authentication, inspect the manager’s isUserAuthenticationEnabled property.

## See Also

### Working with system protection manager

class SystemProtectionManager

A class that represents the status of system protection for the scene.

class let systemProtectionDidChangeNotification: NSNotification.Name

A notification posted when the system-protection attributes of a scene change.

