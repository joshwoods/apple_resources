

- UIKit
- UIApplicationShortcutItem
-  localizedSubtitle 

Instance Property

# localizedSubtitle

The optional, user-visible subtitle for the Home Screen dynamic quick action.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var localizedSubtitle: String? { get }
```

## Discussion

If you specify a subtitle for a quick action, the system then displays the title on a single line (potentially with an ellipsis character), no matter how long the title is.

To internationalize the subtitle for a Home Screen dynamic quick action, employ the NSLocalizedString Foundation function, described in Foundation Functions, along with a `Localized.strings` file in your Xcode project.

## See Also

### Inspecting a Home Screen dynamic quick action

var localizedTitle: String

The required, user-visible title for the Home Screen dynamic quick action.

var type: String

A required, app-specific string that you employ to identify the type of quick action to perform.

var icon: UIApplicationShortcutIcon?

The optional icon for the Home Screen dynamic quick action.

var userInfo: [String : any NSSecureCoding]?

Optional, app-specific information that you can provide for use when your app performs the Home screen quick action.

