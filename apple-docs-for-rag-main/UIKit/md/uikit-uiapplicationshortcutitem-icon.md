

- UIKit
- UIApplicationShortcutItem
-  icon 

Instance Property

# icon

The optional icon for the Home Screen dynamic quick action.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@NSCopying
var icon: UIApplicationShortcutIcon? { get }
```

## Discussion

Quick action icons are template (alpha-channel-only) images that you typically provide as part of an asset catalog. For more information, see UIApplicationShortcutIcon.

## See Also

### Inspecting a Home Screen dynamic quick action

var localizedTitle: String

The required, user-visible title for the Home Screen dynamic quick action.

var localizedSubtitle: String?

The optional, user-visible subtitle for the Home Screen dynamic quick action.

var type: String

A required, app-specific string that you employ to identify the type of quick action to perform.

var userInfo: [String : any NSSecureCoding]?

Optional, app-specific information that you can provide for use when your app performs the Home screen quick action.

