

- UIKit
- UISceneSession
-  configuration 

Instance Property

# configuration

The configuration data for creating the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var configuration: UISceneConfiguration { get }
```

## Discussion

Before the creation of a scene, UIKit creates a UISceneConfiguration object and fills it with details from your app’s `Info.plist` file. (Normally, UIKit chooses the first scene of the appropriate type listed in your scene configuration data.) If the application(_:configurationForConnecting:options:) method of your app delegate returns a new UISceneConfiguration object, UIKit copies that object to this property.

## See Also

### Getting the scene configuration details

class UISceneConfiguration

Information about the objects and storyboard for UKit to use when creating a particular scene.

