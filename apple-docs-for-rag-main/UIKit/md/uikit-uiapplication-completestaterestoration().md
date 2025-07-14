

- UIKit
- UIApplication
-  completeStateRestoration() 

Instance Method

# completeStateRestoration()

Tells the app that your code has finished any asynchronous state restoration.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func completeStateRestoration()
```

## Discussion

UIKit restores your app’s state synchronously on the main thread. If you choose to perform additional state restoration on a secondary thread, call the extendStateRestoration() method to inform UIKit of that fact. Call this method after you finish with your background work to let the system know that state restoration is complete.

## See Also

### Managing state restoration

func extendStateRestoration()

Tells the app that your code is restoring state asynchronously.

func ignoreSnapshotOnNextApplicationLaunch()

Prevents the app from using the recent snapshot image during the next launch cycle.

class func registerObject(forStateRestoration: any UIStateRestoring, restorationIdentifier: String)

Registers a custom object for use with the state restoration system.

