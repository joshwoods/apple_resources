

- ActivityKit
- ActivityUIDismissalPolicy
-  default 

Type Property

# default

The system’s default dismissal policy for the Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
static let `default`: ActivityUIDismissalPolicy
```

## Mentioned in 

Displaying live data with Live Activities

## Discussion

With the default dismissal policy, the system keeps a Live Activity that ended on the Lock Screen for up to four hours after it ends or a person removes it. The ActivityState doesn’t change to ActivityState.dismissed until a person or the system removes the Live Activity user interface.

## See Also

### Dismissing a Live Activity

static let immediate: ActivityUIDismissalPolicy

The system immediately removes the Live Activity that ended.

static func after(Date) -> ActivityUIDismissalPolicy

The system removes the Live Activity that ended at the specified time within a four-hour window.

