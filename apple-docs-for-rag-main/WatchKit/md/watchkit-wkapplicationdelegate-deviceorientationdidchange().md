

- WatchKit
- WKApplicationDelegate
-  deviceOrientationDidChange() 

Instance Method

# deviceOrientationDidChange()

Tells the delegate that the device’s orientation has changed.

watchOS 7.0+

``` source
@MainActor
optional func deviceOrientationDidChange()
```

## Discussion

WatchKit calls this method when the WKInterfaceDevice object’s wristLocation, crownOrientation, or isAutorotated properties change.

## See Also

### Related Documentation

var isAutorotating: Bool

A Boolean value that determines whether the interface automatically rotates when the user flips their wrist.

var isAutorotated: Bool

A Boolean value that indicates whether the system has automatically rotated the user interface so that it is properly oriented for another viewer.

### Monitoring state changes

Working with the watchOS app life cycle

Learn how the watchOS app life cycle operates and responds to life cycle notification methods.

static func main()

Provides the top-level entry point for an app.

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

