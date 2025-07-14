

- UIKit
- UIViewController
-  supportedInterfaceOrientations 

Instance Property

# supportedInterfaceOrientations

The interface orientations that the view controller supports.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var supportedInterfaceOrientations: UIInterfaceOrientationMask { get }
```

## Discussion

This property returns a bit mask that specifies which orientations the view controller supports. For more information, see UIInterfaceOrientationMask.

When the device orientation changes, the system calls this method on the root view controller or the topmost modal view controller that fills the window. If the view controller supports the new orientation, the system rotates the window and the view controller. The system only calls this method if the view controller’s shouldAutorotate method returns true.

Override this method to declare which orientations the view controller supports. The default value is all for the iPad idiom and allButUpsideDown for the iPhone idiom. The value you return must not be 0.

To determine whether to rotate, the system compares the view controller’s supported orientations with the app’s supported orientations — as determined by the `Info.plist` file or the app delegate’s application(_:supportedInterfaceOrientationsFor:) method — and the device’s supported orientations.

Note

All iPadOS devices support the portraitUpsideDown orientation. It’s best practice to enable it for the iPad idiom. iOS devices without a Home button, such as iPhone 12, don’t support this orientation. You should disable it entirely for the iPhone idiom.

If your app supports multitasking, the system doesn’t call this method on your view controller because multitasking apps must support all orientations. You can opt out of multitasking by enabling *Requires full screen* on your iOS target or by not declaring support for all possible orientations within the `Info.plist` file.

For design guidance, see Adaptivity and Layout in the iOS Human Interface Guidelines.

## See Also

### Configuring the view rotation settings

var preferredInterfaceOrientationForPresentation: UIInterfaceOrientation

The interface orientation to use when presenting the view controller.

func setNeedsUpdateOfSupportedInterfaceOrientations()

Notifies the view controller about a change in supported interface orientations or preferred interface orientation for presentation.

