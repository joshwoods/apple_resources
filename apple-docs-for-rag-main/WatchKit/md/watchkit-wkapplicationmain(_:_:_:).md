

- WatchKit
-  WKApplicationMain(\_:\_:\_:) 

Function

# WKApplicationMain(\_:\_:\_:)

Creates the application object and the application delegate, and sets up the app’s event cycle.

watchOS 7.0+

``` source
func WKApplicationMain(
    _ argc: Int32,
    _ argv: UnsafeMutablePointer?>,
    _ applicationDelegateClassName: String?
) -> Int32
```

## Parameters 

`argc`  

The count of arguments in `argv`. This is usually the corresponding parameter to `main`.

`argv`  

A variable list of arguments. This is usually the corresponding parameter to `main`.

`applicationDelegateClassName`  

The name of the app delegate’s class. This class must subclass NSObject and adopt the WKApplicationDelegate protocol.

## Return Value

Even though this function specifies an integer return type, it never returns. When the user exits a watchOS app, the app moves to the background.

## Discussion

This function instantiates the application object and the specified delegate (if any), and then sets the delegate for the application. It also sets up the main event loop, including the application’s run loop, and begins processing events.

## See Also

### App structure

Setting up a watchOS project

Create a new watchOS project or add a watch target to an existing iOS project.

class WKApplication

The centralized point of control and coordination for apps with a single watchOS app target.

protocol WKApplicationDelegate

A collection of methods that manages the app-level behavior for a single-target watchOS app.

class WKExtension

The centralized point of control and coordination for extension-based apps running in watchOS.

protocol WKExtensionDelegate

A collection of methods that manages the app-level behavior of a WatchKit extension.

class WKInterfaceDevice

An object that provides information about the user’s Apple Watch.

WKPrefersNetworkUponForeground

A Boolean value that indicates whether an app requires network access on launch.

