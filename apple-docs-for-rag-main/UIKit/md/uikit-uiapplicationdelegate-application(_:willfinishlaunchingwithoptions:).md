

- UIKit
- UIApplicationDelegate
-  application(\_:willFinishLaunchingWithOptions:) 

Instance Method

# application(\_:willFinishLaunchingWithOptions:)

Tells the delegate that the launch process has begun.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    willFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey : Any]? = nil
) -> Bool
```

## Parameters 

`application`  

The singleton app object.

`launchOptions`  

A dictionary indicating the reason the person or system launched the app. The contents of this dictionary may be empty in situations where a person launched the app directly. If the app supports scenes, this is `nil`. For information about the possible keys in this dictionary and how to handle them, see UIApplication.LaunchOptionsKey.

## Return Value

Return false if the app can’t handle the URL resource or continue a user activity, or if the app doesn’t need to perform the application(_:performActionFor:completionHandler:) method because you’re handling the invocation of a Home Screen quick action in this method; otherwise return true. The system ignores the return value if the app launches as a result of a remote notification.

## Mentioned in 

About the app launch sequence

Performing one-time setup for your app

## Discussion

Use this method (and the corresponding application(_:didFinishLaunchingWithOptions:) method) to initialize your app and prepare it to run. In an app that doesn’t support scenes, the system calls this method after your app launches and loads its main storyboard or nib file, but before restoring your app’s state. When the system calls this method, your app is in the inactive state.

If the system launched your app for a specific reason, the `launchOptions` dictionary contains data indicating the reason for the launch. For some launch reasons, the system may call additional methods of your app delegate. For example, if your app launched to open a URL, the system calls the application(_:open:options:) method after your app finishes initializing itself. The presence of the launch keys gives you the opportunity to plan for that behavior. In the case of a URL to open, you might want to prevent state restoration if the URL represents a document that the person wanted to open.

When the system asks to open a URL, the system combines the return result from this method with the return result from the application(_:didFinishLaunchingWithOptions:) method to determine whether to handle a URL. If either method returns false, the system doesn’t call the application(_:open:options:) method. If you don’t implement one of the methods, the system only considers the return value of the implemented method.

In some cases, a person launches your app with a Home Screen quick action. To ensure you handle this launch case correctly, read the discussion in the application(_:performActionFor:completionHandler:) method.

Important

If your app relies on the state restoration machinery to restore its view controllers, always show your app’s window from this method. Do not show the window in your app’s application(_:didFinishLaunchingWithOptions:) method. Calling the window’s makeKeyAndVisible() method does not make the window visible right away anyway. UIKit waits until your app’s application(_:didFinishLaunchingWithOptions:) method finishes before making the window visible on the screen.

## See Also

### Initializing the app

func application(UIApplication, didFinishLaunchingWithOptions: [UIApplication.LaunchOptionsKey : Any]?) -> Bool

Tells the delegate that the launch process is almost done and the app is almost ready to run.

struct LaunchOptionsKey

The keys you use to access values in the launch options dictionary that the system passes to your app at initialization.

class let didFinishLaunchingNotification: NSNotification.Name

A notification that posts immediately after the app finishes launching.

