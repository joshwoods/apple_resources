

- UIKit
- UIApplication
-  delegate 

Instance Property

# delegate

The delegate of the app object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
unowned(unsafe) var delegate: (any UIApplicationDelegate)? { get set }
```

## Discussion

Every app must have an app delegate object to respond to app-related messages. For example, the app notifies its delegate when the app finishes launching and when its foreground or background execution status changes. Similarly, app-related messages coming from the system are often routed to the app delegate for handling. Xcode provides an initial app delegate for every app and you should not need to change this delegate later.

The delegate must adopt the UIApplicationDelegate formal protocol.

## See Also

### Configuring your app’s behavior

protocol UIApplicationDelegate

A set of methods to manage shared behaviors for your app.

