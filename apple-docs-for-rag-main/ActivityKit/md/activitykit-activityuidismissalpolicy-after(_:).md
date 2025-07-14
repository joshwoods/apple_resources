

- ActivityKit
- ActivityUIDismissalPolicy
-  after(\_:) 

Type Method

# after(\_:)

The system removes the Live Activity that ended at the specified time within a four-hour window.

iOS 16.1+iPadOS 16.1+

``` source
static func after(_ date: Date) -> ActivityUIDismissalPolicy
```

## Parameters 

`date`  

A date within a four-hour window from the moment the Live Activity ends.

## Mentioned in 

Displaying live data with Live Activities

## Discussion

Provide a date to tell the system when it should remove a Live Activity that ended. While you can provide any date, the system removes a Live Activity that ended after the specified date or after four hours from the moment the Live Activity ended — whichever comes first. When the system removes the Live Activity, the ActivityState changes to ActivityState.dismissed.

## See Also

### Dismissing a Live Activity

static let `default`: ActivityUIDismissalPolicy

The system’s default dismissal policy for the Live Activity.

static let immediate: ActivityUIDismissalPolicy

The system immediately removes the Live Activity that ended.

