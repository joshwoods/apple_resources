

- UIKit
- UIApplicationShortcutItem
-  userInfo 

Instance Property

# userInfo

Optional, app-specific information that you can provide for use when your app performs the Home screen quick action.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var userInfo: [String : any NSSecureCoding]? { get }
```

## Discussion

The keys and values in this property’s dictionary must conform to the NSSecureCoding protocol, and must be property-list-encodable. If they aren’t, the system raises a runtime exception when initializing the quick action. For information about property-list-encodable data, see Serializing Property Lists in Archives and Serializations Programming Guide and see PropertyListSerialization.

## See Also

### Inspecting a Home Screen dynamic quick action

var localizedTitle: String

The required, user-visible title for the Home Screen dynamic quick action.

var localizedSubtitle: String?

The optional, user-visible subtitle for the Home Screen dynamic quick action.

var type: String

A required, app-specific string that you employ to identify the type of quick action to perform.

var icon: UIApplicationShortcutIcon?

The optional icon for the Home Screen dynamic quick action.

