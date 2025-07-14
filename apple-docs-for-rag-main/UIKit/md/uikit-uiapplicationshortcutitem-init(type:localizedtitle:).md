

- UIKit
- UIApplicationShortcutItem
-  init(type:localizedTitle:) 

Initializer

# init(type:localizedTitle:)

Creates an immutable Home Screen dynamic quick action with a user-visible title and no icon.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
convenience init(
    type: String,
    localizedTitle: String
)
```

## Parameters 

`type`  

The required, app-defined type of the Home Screen quick action.

`localizedTitle`  

The required, user-visible title of the Home Screen quick action.

## Return Value

An immutable Home Screen dynamic quick action with a user-visible title and no icon.

## See Also

### Creating a Home Screen dynamic quick action

init(type: String, localizedTitle: String, localizedSubtitle: String?, icon: UIApplicationShortcutIcon?, userInfo: [String : any NSSecureCoding]?)

Creates an immutable Home Screen dynamic quick action with user-visible title, icon, and user info dictionary.

