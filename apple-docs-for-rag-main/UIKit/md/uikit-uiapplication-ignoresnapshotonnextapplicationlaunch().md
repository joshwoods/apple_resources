

- UIKit
- UIApplication
-  ignoreSnapshotOnNextApplicationLaunch() 

Instance Method

# ignoreSnapshotOnNextApplicationLaunch()

Prevents the app from using the recent snapshot image during the next launch cycle.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func ignoreSnapshotOnNextApplicationLaunch()
```

## Discussion

As part of the state preservation process, UIKit captures your app’s user interface and stores it in an image file. When your app is relaunched, the system displays this snapshot image in place of your app’s default launch image to preserve the notion that your app was still running. If you feel that the snapshot cannot correctly reflect your app’s user interface when your app is relaunched, call this method to let UIKit know that it should use your app’s default launch image instead of the snapshot.

You must call this method from within the code you use to preserve your app’s state.

## See Also

### Managing state restoration

func extendStateRestoration()

Tells the app that your code is restoring state asynchronously.

func completeStateRestoration()

Tells the app that your code has finished any asynchronous state restoration.

class func registerObject(forStateRestoration: any UIStateRestoring, restorationIdentifier: String)

Registers a custom object for use with the state restoration system.

