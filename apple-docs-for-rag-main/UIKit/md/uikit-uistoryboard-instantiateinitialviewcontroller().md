

- UIKit
- UIStoryboard
-  instantiateInitialViewController() 

Instance Method

# instantiateInitialViewController()

Creates the initial view controller and initializes it with the data from the storyboard.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func instantiateInitialViewController() -> UIViewController?
```

## Return Value

The initial view controller in the storyboard.

## Discussion

Every storyboard file has an initial view controller that represents the default view controller to create. Typically, you use the initial view controller as the root view controller for a window. However, you can also instantiate the initial view controller when transitioning to content in a new storyboard file. This method creates a new instance of the initial view controller using its init(coder:) method.

When you specify a storyboard in the UISceneStoryboardFile or UIMainStoryboardFile key of your app’s `Info.plist` file, UIKit loads the initial view controller from that storyboard.

## See Also

### Loading the Initial View Controller

func instantiateInitialViewController&lt;ViewController>(creator: ((NSCoder) -> ViewController?)?) -> ViewController?

Creates the initial view controller from the storyboard and initializes it using your custom initialization code.

