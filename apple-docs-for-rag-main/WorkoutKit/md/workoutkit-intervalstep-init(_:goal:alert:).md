

- WorkoutKit
- IntervalStep
-  init(\_:goal:alert:) 

Initializer

# init(\_:goal:alert:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

**iOS, iPadOS**

``` source
init(
    _ purpose: IntervalStep.Purpose,
    goal: WorkoutGoal = .open,
    alert: (WorkoutAlert)? = nil
)
```

**Mac Catalyst, macOS, watchOS**

``` source
init(
    _ purpose: IntervalStep.Purpose,
    goal: WorkoutGoal = .open,
    alert: (any WorkoutAlert)? = nil
)
```

## See Also

### Creating interval steps

init(IntervalStep.Purpose, step: WorkoutStep)

Creates a new interval step.

