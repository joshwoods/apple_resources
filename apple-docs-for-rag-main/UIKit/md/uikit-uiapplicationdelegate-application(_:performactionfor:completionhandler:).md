

- UIKit
- UIApplicationDelegate
-  application(\_:performActionFor:completionHandler:) 

Instance Method

# application(\_:performActionFor:completionHandler:)

Tells the delegate that the user selected a Home screen quick action for your app, except when you’ve intercepted the interaction in a launch method.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    performActionFor shortcutItem: UIApplicationShortcutItem,
    completionHandler: @escaping (Bool) -> Void
)
```

``` source
@MainActor
optional func application(
    _ application: UIApplication,
    performActionFor shortcutItem: UIApplicationShortcutItem
) async -> Bool
```

## Parameters 

`application`  

Your shared app object.

`shortcutItem`  

The quick action for which you’re providing an implementation in this method.

`completionHandler`  

The block you call after your quick action implementation completes, returning true or false depending on the success or failure of your implementation code.

succeeded  
A Boolean value that indicates whether or not your implementation succeeded.

## Discussion

Important

This method is not called for scene-based apps. If you have a scene-based app, implement windowScene(_:performActionFor:completionHandler:) in your scene delegate instead.

Implement this method to respond to the user’s selection of a Home screen quick action for your app. When finished, call the completion handler, with an appropriate Boolean value.

It’s your responsibility to ensure the system calls this method conditionally, depending on whether or not one of your app launch methods (application(_:willFinishLaunchingWithOptions:) or application(_:didFinishLaunchingWithOptions:)) has already handled a quick action invocation. The system calls a launch method (before calling this method) when a user selects a quick action for your app and your app *launches* instead of *activating*.

The requested quick action might employ code paths different than those used otherwise when your app launches. For example, your app normally launches to display view A, but your app was launched in response to a quick action that needs view B. To handle such cases, upon launch, check whether your app is being launched via a quick action. Perform this check in your application(_:willFinishLaunchingWithOptions:) or application(_:didFinishLaunchingWithOptions:) method by checking for the shortcutItem launch option key. The UIApplicationShortcutItem object is available as the value of the launch option key.

If you find that your app was indeed launched using a quick action, perform the requested quick action within the launch method and return a value of false from that method. When you return a value of false, the system doesn’t call the application(_:performActionFor:completionHandler:) method.

## See Also

### Continuing user activity and handling quick actions

func application(UIApplication, willContinueUserActivityWithType: String) -> Bool

Tells the delegate if your app takes responsibility for notifying users when a continuation activity takes longer than expected.

func application(UIApplication, continue: NSUserActivity, restorationHandler: ([any UIUserActivityRestoring]?) -> Void) -> Bool

Tells the delegate that the data for continuing an activity is available.

func application(UIApplication, didUpdate: NSUserActivity)

Tells the delegate that the activity was updated.

func application(UIApplication, didFailToContinueUserActivityWithType: String, error: any Error)

Tells the delegate that the activity couldn’t be continued.

