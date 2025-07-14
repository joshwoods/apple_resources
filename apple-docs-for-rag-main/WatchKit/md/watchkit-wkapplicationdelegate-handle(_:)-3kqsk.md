

- WatchKit
- WKApplicationDelegate
-  handle(\_:) 

Instance Method

# handle(\_:)

Responds to Handoff–related activity from Siri.

watchOS 7.0+

``` source
@MainActor
optional func handle(_ userActivity: NSUserActivity)
```

## Parameters 

`userActivity`  

The activity object containing the data associated with the task the user was performing. Use the data to continue the user’s activity in your app on Apple Watch.

## Discussion

WatchKit calls this method when it receives data associated with a user activity. Use this method to update your app on Apple Watch so that the user can continue the activity from where they left off.

## See Also

### Coordinating Handoff activity

func handleUserActivity([AnyHashable : Any]?)

Responds to Handoff–related activity from complications and notifications.

