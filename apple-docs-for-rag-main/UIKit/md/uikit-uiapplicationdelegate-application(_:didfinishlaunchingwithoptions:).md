

- UIKit
- UIApplicationDelegate
-  application(\_:didFinishLaunchingWithOptions:) 

Instance Method

# application(\_:didFinishLaunchingWithOptions:)

Tells the delegate that the launch process is almost done and the app is almost ready to run.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey : Any]? = nil
) -> Bool
```

## Parameters 

`application`  

The singleton app object.

`launchOptions`  

A dictionary indicating the reason the person or system launched the app. The contents of this dictionary may be empty in situations where a person launched the app directly. If the app supports scenes, this is `nil`. For information about the possible keys in this dictionary and how to handle them, see UIApplication.LaunchOptionsKey.

## Return Value

Return false if the app can’t handle the URL resource or continue a user activity, otherwise return true. The system ignores the return value if the app launches as a result of a remote notification.

## Mentioned in 

Performing one-time setup for your app

About the app launch sequence

About the UI restoration process

## Discussion

Use this method (and the corresponding application(_:willFinishLaunchingWithOptions:) method) to complete your app’s initialization. In an app that supports scenes:

- The system calls this method as soon as the process is done launching.

- The system then creates the scene(s) that you configured for your app.

- The system calls scene life-cycle methods, such as scene(_:willConnectTo:options:).

- As the system presents a scene, it updates that scene’s activationState. The app’s state is the aggregate of all the scene UIScene.ActivationState values.

In an app that doesn’t support scenes:

- The system performs state restoration before calling this method.

- The system calls this method when the process is done launching.

- The system presents your app’s window, scene(s), and other UI.

- At some point after this method returns, the system calls another of your app delegate’s methods to move the app to the active (foreground) state or the background state.

This method represents your last chance to process any keys in the `launchOptions` dictionary. If you didn’t evaluate the keys in your application(_:willFinishLaunchingWithOptions:) method, review them in this method and provide an appropriate response.

Objects that aren’t the app delegate can access the same `launchOptions` dictionary values by observing the notification named didFinishLaunchingNotification and accessing the notification’s userInfo dictionary. The system sends that notification shortly after this method returns.

The system combines the return result from this method with the return result from the application(_:willFinishLaunchingWithOptions:) method to determine whether to handle a URL. If either method returns false, the system doesn’t handle the URL. If you don’t implement one of the methods, the system only considers the return value of the implemented method.

## See Also

### Related Documentation

func applicationDidEnterBackground(UIApplication)

Tells the delegate that the app is now in the background.

func applicationDidBecomeActive(UIApplication)

Tells the delegate that the app has become active.

### Initializing the app

func application(UIApplication, willFinishLaunchingWithOptions: [UIApplication.LaunchOptionsKey : Any]?) -> Bool

Tells the delegate that the launch process has begun.

struct LaunchOptionsKey

The keys you use to access values in the launch options dictionary that the system passes to your app at initialization.

class let didFinishLaunchingNotification: NSNotification.Name

A notification that posts immediately after the app finishes launching.

