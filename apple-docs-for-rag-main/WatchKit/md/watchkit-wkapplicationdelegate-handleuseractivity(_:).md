

- WatchKit
- WKApplicationDelegate
-  handleUserActivity(\_:) 

Instance Method

# handleUserActivity(\_:)

Responds to Handoff–related activity from complications and notifications.

watchOS 7.0+

``` source
@MainActor
optional func handleUserActivity(_ userInfo: [AnyHashable : Any]?)
```

## Parameters 

`userInfo`  

The dictionary containing data about the activity.

## Discussion

Use this method to respond to Handoff–related activity. WatchKit calls this method when your app launches as a result of a Handoff action. Use the information in the provided `userInfo` dictionary to determine how you want to respond to the action. For example, you might decide to display a specific view.

The default implementation of this method does nothing. When overriding this method, don’t call `super`.

Note

If you’re creating a SwiftUI app for watchOS 7 or later, use the onContinueUserActivity(_:perform:) modifier instead.

## See Also

### Related Documentation

func updateUserActivity(String, userInfo: [AnyHashable : Any]?, webpageURL: URL?)

Registers the current user activity with the system.

Deprecated

### Coordinating Handoff activity

func handle(NSUserActivity)

Responds to Handoff–related activity from Siri.

