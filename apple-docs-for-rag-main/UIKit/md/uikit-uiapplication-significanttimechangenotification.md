

- UIKit
- UIApplication
-  significantTimeChangeNotification 

Type Property

# significantTimeChangeNotification

A notification that posts when there’s a significant change in time.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
nonisolated
class let significantTimeChangeNotification: NSNotification.Name
```

## Mentioned in 

Processing queued notifications

## Discussion

The system posts this notification when, for example, there’s a change to a new day (midnight), a carrier time update, or a change to, or from, daylight savings time. The notification doesn’t contain a user info dictionary.

## See Also

### Responding to environment changes

func applicationProtectedDataDidBecomeAvailable(UIApplication)

Tells the delegate that protected files are available now.

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

