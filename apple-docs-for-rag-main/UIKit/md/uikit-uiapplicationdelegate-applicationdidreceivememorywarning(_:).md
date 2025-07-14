

- UIKit
- UIApplicationDelegate
-  applicationDidReceiveMemoryWarning(\_:) 

Instance Method

# applicationDidReceiveMemoryWarning(\_:)

Tells the delegate when the app receives a memory warning from the system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func applicationDidReceiveMemoryWarning(_ application: UIApplication)
```

## Parameters 

`application`  

Your singleton app object.

## Mentioned in 

Responding to memory warnings

## Discussion

Your implementation of this method should free up as much memory as possible by purging cached data objects that can be recreated (or reloaded from disk) later. You use this method in conjunction with the didReceiveMemoryWarning() of the UIViewController class and the didReceiveMemoryWarningNotification notification to release memory throughout your app.

It is strongly recommended that you implement this method. If your app does not release enough memory during low-memory conditions, the system may terminate it outright.

## See Also

### Related Documentation

func didReceiveMemoryWarning()

Sent to the view controller when the app receives a memory warning.

### Responding to environment changes

func applicationProtectedDataDidBecomeAvailable(UIApplication)

Tells the delegate that protected files are available now.

func applicationProtectedDataWillBecomeUnavailable(UIApplication)

Tells the delegate that the protected files are about to become unavailable.

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

