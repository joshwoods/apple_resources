

- UIKit
- UIApplicationShortcutItem
-  init(type:localizedTitle:localizedSubtitle:icon:userInfo:) 

Initializer

# init(type:localizedTitle:localizedSubtitle:icon:userInfo:)

Creates an immutable Home Screen dynamic quick action with user-visible title, icon, and user info dictionary.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
init(
    type: String,
    localizedTitle: String,
    localizedSubtitle: String?,
    icon: UIApplicationShortcutIcon?,
    userInfo: [String : any NSSecureCoding]? = nil
)
```

## Parameters 

`type`  

The required, app-defined type of the Home Screen quick action.

`localizedTitle`  

The required, user-visible title of the Home Screen quick action.

`localizedSubtitle`  

The optional, user-visible subtitle of the Home Screen quick action.

`icon`  

The optional icon for the Home Screen quick action.

`userInfo`  

App-defined information about the Home Screen quick action, to be used by your app to implement the action.

Important

This method throws an exception if the value of this parameter isn’t property-list-encodable. For more information, see Serializing Property Lists in Archives and Serializations Programming Guide and see PropertyListSerialization.

One common, important use for this dictionary is to specify the version of your app. If a user installs an update for your app but hasn’t yet launched the update, pressing your Home Screen icon shows the dynamic quick actions for the previously-installed version. Including the app version in the `userInfo` dictionary lets you gracefully handle this scenario.

## Return Value

An immutable Home Screen dynamic quick action item with a user-visible title, optional subtitle, optional icon, and optional user info dictionary.

## See Also

### Creating a Home Screen dynamic quick action

convenience init(type: String, localizedTitle: String)

Creates an immutable Home Screen dynamic quick action with a user-visible title and no icon.

