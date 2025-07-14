

- WatchKit
- WKApplication
-  didBecomeActiveNotification 

Type Property

# didBecomeActiveNotification

A message indicating that the watchOS app is visible and processing events.

watchOS 7.0+

``` source
@MainActor @preconcurrency
static let didBecomeActiveNotification: NSNotification.Name
```

## Discussion

When creating an app that uses the SwiftUI App protocol to manage your life cycle, use the onChange(of:perform:) modifier and the scenePhase environment value to monitor life cycle changes when possible. For more information, see Building a watchOS app.

## See Also

### Observing messages from the notification center

static let didFinishLaunchingNotification: NSNotification.Name

A message indicating that the launch process finished and the extension is ready to run.

static let willResignActiveNotification: NSNotification.Name

A message indicating that the system is about to deactivate the watchOS app.

static let willEnterForegroundNotification: NSNotification.Name

A message indicating that the watchOS app is about to transition from the background to the foreground.

static let didEnterBackgroundNotification: NSNotification.Name

A message indicating that the watchOS app transitioned from the foreground to the background.

