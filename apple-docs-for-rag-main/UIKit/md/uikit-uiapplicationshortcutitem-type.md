

- UIKit
- UIApplicationShortcutItem
-  type 

Instance Property

# type

A required, app-specific string that you employ to identify the type of quick action to perform.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var type: String { get }
```

## See Also

### Inspecting a Home Screen dynamic quick action

var localizedTitle: String

The required, user-visible title for the Home Screen dynamic quick action.

var localizedSubtitle: String?

The optional, user-visible subtitle for the Home Screen dynamic quick action.

var icon: UIApplicationShortcutIcon?

The optional icon for the Home Screen dynamic quick action.

var userInfo: [String : any NSSecureCoding]?

Optional, app-specific information that you can provide for use when your app performs the Home screen quick action.

