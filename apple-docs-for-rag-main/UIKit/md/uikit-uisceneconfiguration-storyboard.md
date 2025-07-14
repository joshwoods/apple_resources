

- UIKit
- UISceneConfiguration
-  storyboard 

Instance Property

# storyboard

The storyboard object that contains your scene’s initial view controller.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var storyboard: UIStoryboard? { get set }
```

## Discussion

UIKit loads the initial view controller from the specified scene and displays it appropriately.

UIKit sets this property’s initial value using the UISceneStoryboardFile key from the appropriate scene in your app’s `Info.plist` file.

## See Also

### Specifying the scene creation details

var sceneClass: AnyClass?

The class of the scene object that you want UIKit to create.

var delegateClass: AnyClass?

The class of the custom delegate object that you want UIKit to create.

