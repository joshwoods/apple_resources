

- ClockKit
- CLKComplicationServer
-  activeComplications Deprecated

Instance Property

# activeComplications

The active complications for the current app.

watchOS 2.0–9.0Deprecated

``` source
var activeComplications: [CLKComplication]? { get }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Mentioned in 

Keeping your complications up to date

## Discussion

This property contains an array of CLKComplication objects; each represents a version of your complication currently displayed on the clock face. If the property contains an empty array, it means your app has no complications on the active watch face. If it’s `nil`, it means the server is still connecting to the active complications.

There are no guarantees on when the server will connect with the complications. ClockKit sends a CLKComplicationServerActiveComplicationsDidChangeNotification notification when the server connects, and the system guarantees that the activeComplications property has a non-`nil` value after it sends the notification.

To avoid any race conditions, always perform the following steps in order:

1.  Set up an observer for the CLKComplicationServerActiveComplicationsDidChangeNotification notification.

2.  Check and see if activeComplications contains a `nil` value.

If activeComplications has a non-`nil` value, you can use it immediately. Otherwise, wait for the notification to fire, and then check the activeComplications property again.

The following code listing shows a safe implementation using Swift’s asynchronous APIs.

```
extension CLKComplicationServer {

    // Safely access the server's active complications.
    @MainActor
    func getActiveComplications() async -> [CLKComplication] {
        return await withCheckedContinuation { continuation in

            // First, set up the notification.
            let center = NotificationCenter.default
            let mainQueue = OperationQueue.main
            var token: NSObjectProtocol?
            token = center.addObserver(forName: .CLKComplicationServerActiveComplicationsDidChange, object: nil, queue: mainQueue) { _ in
                center.removeObserver(token!)
                continuation.resume(returning: self.activeComplications!)
            }

            // Then check to see if we have a valid active complications array.
            if activeComplications != nil {
                center.removeObserver(token!)
                continuation.resume(returning: self.activeComplications!)
            }
        }
    }
}
```

