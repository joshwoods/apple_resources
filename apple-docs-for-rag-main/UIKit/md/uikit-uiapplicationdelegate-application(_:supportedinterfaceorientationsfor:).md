

- UIKit
- UIApplicationDelegate
-  application(\_:supportedInterfaceOrientationsFor:) 

Instance Method

# application(\_:supportedInterfaceOrientationsFor:)

Asks the delegate for the interface orientations to use for the view controllers in the specified window.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    supportedInterfaceOrientationsFor window: UIWindow?
) -> UIInterfaceOrientationMask
```

## Parameters 

`application`  

Your singleton app object.

`window`  

The window whose interface orientations you want to retrieve.

## Return Value

A bit mask of the UIInterfaceOrientationMask constants that indicate the orientations to use for the view controllers.

## Discussion

This method returns the total set of interface orientations supported by the app. When determining whether to rotate a particular view controller, the orientations returned by this method are intersected with the orientations supported by the root view controller or topmost presented view controller. The app and view controller must agree before the rotation is allowed.

If you do not implement this method, the app uses the values in the `UIInterfaceOrientation` key of the app’s `Info.plist` as the default interface orientations.

## See Also

### Managing interface geometry

enum UIInterfaceOrientation

Constants that specify the orientation of the app’s user interface.

struct UIInterfaceOrientationMask

Constants that specify a view controller’s supported interface orientations.

class let invalidInterfaceOrientationException: NSExceptionName

An exception that’s thrown if a view controller or the app returns an invalid set of supported interface orientations.

