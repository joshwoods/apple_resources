

- HealthKitUI
- HKActivityRingView
-  activitySummary 

Instance Property

# activitySummary

The active summary displayed by the activity ring view.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
var activitySummary: HKActivitySummary? { get set }
```

## Discussion

Any changes made directly to this property are not animated. To animate changes, use \# setActivitySummary(_:animated:) instead.

## See Also

### Setting the activity summary

func setActivitySummary(HKActivitySummary?, animated: Bool)

Sets the activity summary displayed by the activity ring view.

