

- UIKit
- UIApplication
-  extendStateRestoration() 

Instance Method

# extendStateRestoration()

Tells the app that your code is restoring state asynchronously.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func extendStateRestoration()
```

## Discussion

UIKit restores your app’s state synchronously on the main thread. If you choose to perform additional state restoration on a secondary thread, call this method to inform UIKit of that fact. You must balance each call to this method with a matching call to the completeStateRestoration() method.

Calling this method is a safety precaution in the event that your app crashes at launch time due to problems restoring its state. If you call this method but do not call the matching completeStateRestoration() method before a crash occurs, the system throws away any saved state information. Doing so prevents your app from crashing during subsequent launches because of issues caused by trying to restore your app’s state.

## See Also

### Managing state restoration

func completeStateRestoration()

Tells the app that your code has finished any asynchronous state restoration.

func ignoreSnapshotOnNextApplicationLaunch()

Prevents the app from using the recent snapshot image during the next launch cycle.

class func registerObject(forStateRestoration: any UIStateRestoring, restorationIdentifier: String)

Registers a custom object for use with the state restoration system.

