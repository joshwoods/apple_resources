

- WorkoutKit
- WorkoutAlert
-  supports(activity:location:) 

Instance Method

# supports(activity:location:)

Returns a Boolean value that indicates whether the alert supports the provided activity and location.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
func supports(
    activity: HKWorkoutActivityType,
    location: HKWorkoutSessionLocationType
) -> Bool
```

**Required**

## Parameters 

`activity`  

The workout’s activity type.

`location`  

The workout’s location type.

