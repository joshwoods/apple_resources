

- UIKit
- UIScene
-  systemProtectionDidChangeNotification 

Type Property

# systemProtectionDidChangeNotification

A notification posted when the system-protection attributes of a scene change.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
nonisolated
class let systemProtectionDidChangeNotification: NSNotification.Name
```

## Discussion

The object of the notification is the scene for which protection attributes changed.

## See Also

### Working with system protection manager

var systemProtectionManager: UIScene.SystemProtectionManager?

The system protection manager associated with this scene.

class SystemProtectionManager

A class that represents the status of system protection for the scene.

