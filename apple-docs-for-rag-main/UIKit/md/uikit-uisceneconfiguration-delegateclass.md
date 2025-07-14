

- UIKit
- UISceneConfiguration
-  delegateClass 

Instance Property

# delegateClass

The class of the custom delegate object that you want UIKit to create.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var delegateClass: AnyClass? { get set }
```

## Discussion

If you specified UIWindowScene in the sceneClass property, your delegate class must conform to the UIWindowSceneDelegate protocol. Otherwise, you must specify a class that conforms to the UISceneDelegate protocol.

UIKit sets this property’s initial value using the UISceneDelegateClassName key from the appropriate scene in your app’s `Info.plist` file.

## See Also

### Specifying the scene creation details

var sceneClass: AnyClass?

The class of the scene object that you want UIKit to create.

var storyboard: UIStoryboard?

The storyboard object that contains your scene’s initial view controller.

