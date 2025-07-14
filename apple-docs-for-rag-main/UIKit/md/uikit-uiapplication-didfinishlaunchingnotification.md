

- UIKit
- UIApplication
-  didFinishLaunchingNotification 

Type Property

# didFinishLaunchingNotification

A notification that posts immediately after the app finishes launching.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
nonisolated
class let didFinishLaunchingNotification: NSNotification.Name
```

## Discussion

If the app was launched as a result of in remote notification targeted at it or because another app opened a URL resource claimed the posting app (the notification `object`), this notification contains a `userInfo` dictionary. You can access the contents of the dictionary using the url and sourceApplication constants (for URLs), the remoteNotification constant (for remote notifications), and the localNotification constant (for local notifications). If the notification was posted for a normal app launch, there is no `userInfo` dictionary.

## See Also

### Initializing the app

func application(UIApplication, willFinishLaunchingWithOptions: [UIApplication.LaunchOptionsKey : Any]?) -> Bool

Tells the delegate that the launch process has begun.

func application(UIApplication, didFinishLaunchingWithOptions: [UIApplication.LaunchOptionsKey : Any]?) -> Bool

Tells the delegate that the launch process is almost done and the app is almost ready to run.

struct LaunchOptionsKey

The keys you use to access values in the launch options dictionary that the system passes to your app at initialization.

