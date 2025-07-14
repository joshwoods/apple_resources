

- HealthKitUI
- HKActivityRingView
-  setActivitySummary(\_:animated:) 

Instance Method

# setActivitySummary(\_:animated:)

Sets the activity summary displayed by the activity ring view.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
func setActivitySummary(
    _ activitySummary: HKActivitySummary?,
    animated: Bool
)
```

## Parameters 

`activitySummary`  

The new activity summary.

`animated`  

If true, the change is animated.

## See Also

### Setting the activity summary

var activitySummary: HKActivitySummary?

The active summary displayed by the activity ring view.

