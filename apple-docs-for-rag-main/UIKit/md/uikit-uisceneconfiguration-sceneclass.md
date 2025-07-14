

- UIKit
- UISceneConfiguration
-  sceneClass 

Instance Property

# sceneClass

The class of the scene object that you want UIKit to create.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var sceneClass: AnyClass? { get set }
```

## Discussion

The class you specify must be UIScene or one of its subclasses. Typically, you specify the UIWindowScene class for all windows associated with your app.

UIKit sets this property’s initial value using the UISceneClassName key from the appropriate scene in your app’s `Info.plist` file.

## See Also

### Specifying the scene creation details

var delegateClass: AnyClass?

The class of the custom delegate object that you want UIKit to create.

var storyboard: UIStoryboard?

The storyboard object that contains your scene’s initial view controller.

