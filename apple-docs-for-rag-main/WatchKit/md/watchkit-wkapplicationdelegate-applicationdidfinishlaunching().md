

- WatchKit
- WKApplicationDelegate
-  applicationDidFinishLaunching() 

Instance Method

# applicationDidFinishLaunching()

Tells the delegate that the launch process is almost done and the app is almost ready to run.

watchOS 7.0+

``` source
@MainActor
optional func applicationDidFinishLaunching()
```

## Discussion

WatchKit calls this method after the launch cycle has finished and before your app’s interface is active. Use this method to complete your watchOS apps initialization and prepare it to run. For example, a page-based app could use this method to call the reloadRootControllers(withNames:contexts:) method to specify the initial set of interface controllers to display.

Note

When creating an app that uses the SwiftUI App protocol to manage your life cycle, use the onChange(of:perform:) modifier and the scenePhase environment value to monitor life cycle changes when possible. For more information, see Building a watchOS app.

## See Also

### Monitoring state changes

Working with the watchOS app life cycle

Learn how the watchOS app life cycle operates and responds to life cycle notification methods.

static func main()

Provides the top-level entry point for an app.

func applicationDidBecomeActive()

Tells the delegate that the watchOS app is visible and processing events.

func applicationWillResignActive()

Tells the delegate that the system is about to deactivate the watchOS app.

func applicationWillEnterForeground()

Tells the delegate that the app is about to transition from the background to the foreground.

func applicationDidEnterBackground()

Tells the delegate that the app has transitioned from the foreground to the background.

func deviceOrientationDidChange()

Tells the delegate that the device’s orientation has changed.

