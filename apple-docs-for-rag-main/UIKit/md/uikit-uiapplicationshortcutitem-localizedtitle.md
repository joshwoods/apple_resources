

- UIKit
- UIApplicationShortcutItem
-  localizedTitle 

Instance Property

# localizedTitle

The required, user-visible title for the Home Screen dynamic quick action.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var localizedTitle: String { get }
```

## Discussion

Every Home Screen dynamic quick action must have a user-visible title.

If the title fits on one line, the system displays it as a single line quick action. If the title is too long for one line and you have not specified a localizedSubtitle string, the system displays the title on two lines.

To internationalize the title for a Home Screen dynamic quick action, employ the NSLocalizedString Foundation function, described in Foundation Functions, along with a `Localizable.strings` file in your Xcode project.

## See Also

### Inspecting a Home Screen dynamic quick action

var localizedSubtitle: String?

The optional, user-visible subtitle for the Home Screen dynamic quick action.

var type: String

A required, app-specific string that you employ to identify the type of quick action to perform.

var icon: UIApplicationShortcutIcon?

The optional icon for the Home Screen dynamic quick action.

var userInfo: [String : any NSSecureCoding]?

Optional, app-specific information that you can provide for use when your app performs the Home screen quick action.

