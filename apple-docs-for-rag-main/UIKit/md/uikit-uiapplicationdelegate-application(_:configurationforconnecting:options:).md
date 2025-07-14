

- UIKit
- UIApplicationDelegate
-  application(\_:configurationForConnecting:options:) 

Instance Method

# application(\_:configurationForConnecting:options:)

Retrieves the configuration data for UIKit to use when creating a new scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    configurationForConnecting connectingSceneSession: UISceneSession,
    options: UIScene.ConnectionOptions
) -> UISceneConfiguration
```

## Parameters 

`application`  

The singleton app object.

`connectingSceneSession`  

The session object associated with the scene. This object contains the initial configuration data loaded from the app’s `Info.plist` file, if any.

`options`  

System-specific options for configuring the scene.

## Return Value

The configuration object containing the information needed to create the scene.

## Mentioned in 

Specifying the scenes your app supports

## Discussion

Implement this method if you don’t include scene-configuration data in your app’s `Info.plist` file, or if you want to alter the scene configuration data dynamically. UIKit calls this method shortly before creating a new scene. In your implementation, return a UISceneConfiguration object with the scene details, including the type of scene to create, the delegate object you use to manage the scene, and the storyboard containing the initial view controller to display.

If you don’t implement this method, you must provide scene-configuration data in your app’s `Info.plist` file.

## See Also

### Configuring and discarding scenes

func application(UIApplication, didDiscardSceneSessions: Set&lt;UISceneSession>)

Tells the delegate that the user closed one or more of the app’s scenes from the app switcher.

