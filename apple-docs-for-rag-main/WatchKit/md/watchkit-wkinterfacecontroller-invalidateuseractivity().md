

- WatchKit
- WKInterfaceController
-  invalidateUserActivity() 

Instance Method

# invalidateUserActivity()

Invalidates the most recent user activity.

watchOS 2.0+

``` source
@MainActor
func invalidateUserActivity()
```

## Discussion

Use this method to invalidate an activity that should no longer be performed.

## See Also

### Coordinating Handoff activity

func update(NSUserActivity)

Registers the current user activity with the system.

