

- UIKit
- UIApplicationDelegate
-  applicationProtectedDataDidBecomeAvailable(\_:) 

Instance Method

# applicationProtectedDataDidBecomeAvailable(\_:)

Tells the delegate that protected files are available now.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func applicationProtectedDataDidBecomeAvailable(_ application: UIApplication)
```

## Parameters 

`application`  

Your singleton app object.

## Mentioned in 

Encrypting Your App’s Files

## Discussion

On a device that uses content protection, protected files are stored in an encrypted form and made available only at certain times, usually when the device is unlocked. This notification lets your app know that the device is now unlocked and that you may access certain types of protected files again.

## See Also

### Responding to environment changes

func applicationProtectedDataWillBecomeUnavailable(UIApplication)

Tells the delegate that the protected files are about to become unavailable.

func applicationDidReceiveMemoryWarning(UIApplication)

Tells the delegate when the app receives a memory warning from the system.

func applicationSignificantTimeChange(UIApplication)

Tells the delegate when there is a significant change in the time.

class let protectedDataDidBecomeAvailableNotification: NSNotification.Name

A notification that posts when the protected files become available for your code to access.

class let protectedDataWillBecomeUnavailableNotification: NSNotification.Name

A notification that posts shortly before protected files are locked down and become inaccessible.

class let didReceiveMemoryWarningNotification: NSNotification.Name

A notification that posts when the app receives a warning from the operating system about low memory availability.

class let significantTimeChangeNotification: NSNotification.Name

A notification that posts when there’s a significant change in time.

