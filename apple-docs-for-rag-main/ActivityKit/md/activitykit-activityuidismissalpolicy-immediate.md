

- ActivityKit
- ActivityUIDismissalPolicy
-  immediate 

Type Property

# immediate

The system immediately removes the Live Activity that ended.

iOS 16.1+iPadOS 16.1+

``` source
static let immediate: ActivityUIDismissalPolicy
```

## Mentioned in 

Displaying live data with Live Activities

## Discussion

With the `immediate` dismissal policy, the system immediately removes the ended Live Activity and the ActivityState changes to ActivityState.dismissed.

## See Also

### Dismissing a Live Activity

static let `default`: ActivityUIDismissalPolicy

The system’s default dismissal policy for the Live Activity.

static func after(Date) -> ActivityUIDismissalPolicy

The system removes the Live Activity that ended at the specified time within a four-hour window.

