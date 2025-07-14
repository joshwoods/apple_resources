

- UIKit
- UIScene
- UIScene.SystemProtectionManager
-  isUserAuthenticationEnabled 

Instance Property

# isUserAuthenticationEnabled

The current status of system user authentication.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor
var isUserAuthenticationEnabled: Bool { get }
```

## Discussion

This value is `true` if the system requires device owner authentication challenges to reveal the content of the scene associated with this manager, `false` otherwise.

Note

This value represents whether protection is enabled in general. It doesn’t indicate the instantaneous state of whether any system-provided shield covers the UI at the moment.

