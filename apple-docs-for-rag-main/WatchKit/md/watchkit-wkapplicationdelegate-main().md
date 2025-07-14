

- WatchKit
- WKApplicationDelegate
-  main() 

Type Method

# main()

Provides the top-level entry point for an app.

watchOS 7.0+

``` source
@MainActor @preconcurrency
static func main()
```

## Discussion

WKApplicationDelegate provides an implementation of the main() method that serves as the main entry point for your watchOS app. The system calls the main() method to launch your app; you never call it yourself. Your app can have exactly one entry point, which you mark with the `@main` attribute.

## See Also

### Monitoring state changes

Working with the watchOS app life cycle

Learn how the watchOS app life cycle operates and responds to life cycle notification methods.

func applicationDidFinishLaunching()

Tells the delegate that the launch process is almost done and the app is almost ready to run.

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

