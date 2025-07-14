

- WatchKit
- WKExtensionDelegate
-  handleUserActivity(\_:) 

Instance Method

# handleUserActivity(\_:)

Responds to Handoff–related activity from complications and notifications.

watchOS 2.0+

``` source
@MainActor
optional func handleUserActivity(_ userInfo: [AnyHashable : Any]?)
```

## Parameters 

`userInfo`  

The dictionary containing data about the activity.

## Discussion

Use this method to respond to Handoff–related activity. WatchKit calls this method when your app launches as a result of a Handoff action. Use the information in the provided `userInfo` dictionary to determine how you want to respond to the action. For example, you might decide to display a specific interface controller.

The default implementation of this method does nothing. When overriding this method, don’t call `super`.

Note

If you are creating a SwiftUI app for watchOS 7 or later, use the onContinueUserActivity(_:perform:) modifier instead.

### Handling Activities from Complications and Notifications

WatchKit calls this method when your app launches from a complication or notification. Update your app’s user interface based on the `userInfo` parameter. Your app should seamlessly continue the interaction from the complication or notification.

When your app launches because the user tapped on a complication, the `userInfo` dictionary contains the CLKLaunchedTimelineEntryDateKey key. The value is a Date object that indicates when the complication launched.

## See Also

### Related Documentation

func updateUserActivity(String, userInfo: [AnyHashable : Any]?, webpageURL: URL?)

Registers the current user activity with the system.

Deprecated

### Coordinating handoff activity

func handle(NSUserActivity)

Responds to Handoff–related activity from Siri.

