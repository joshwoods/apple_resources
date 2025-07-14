

- WorkoutKit
- WorkoutPlan
-  init(\_:id:) 

Initializer

# init(\_:id:)

Creates a new workout plan from the provided workout and ID.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(
    _ workout: WorkoutPlan.Workout,
    id: UUID = UUID()
)
```

## Parameters 

`workout`  

The workout represented by this plan.

`id`  

A unique ID for the plan.

## See Also

### Creating a workout plan

enum Workout

The workout for the workout plan.

