

- UIKit
- UISceneConfiguration
-  init(name:sessionRole:) 

Initializer

# init(name:sessionRole:)

Creates a scene-configuration object with the specified role and app-specific name.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(
    name: String?,
    sessionRole: UISceneSession.Role
)
```

## Parameters 

`name`  

The app-specific name you want to assign to the scene. For scenes you specify in your Info.plist file, this value corresponds to the string assigned to the UISceneConfigurationName key.

`sessionRole`  

The role of the scene. For a list of possible roles, see UISceneSession.Role.

## Return Value

A new scene-configuration object.

## Discussion

After creating a scene-configuration object, supply values for the sceneClass, delegateClass, and storyboard properties.

