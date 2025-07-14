

- WatchKit
- WKExtensionDelegate
-  handle(\_:) 

Instance Method

# handle(\_:)

Tells the delegate that the user started a workout session on the paired iPhone.

watchOS 3.0+

``` source
@MainActor
optional func handle(_ workoutConfiguration: HKWorkoutConfiguration)
```

## Parameters 

`workoutConfiguration`  

The workout configuration data. You can use this information to start a workout session on the user’s Apple Watch.

## Discussion

When your iPhone app starts a workout session using the HealthKit store’s `startWatchAppWithWorkoutConfiguration:completion:` method, the system launches or wakes the corresponding Watch app in the background and calls this method. Use this method to configure an HKWorkoutSession object in your Watch app, and then call start(_:) to start the session.

## See Also

### Handling a workout session

func handleActiveWorkoutRecovery()

Tells the delegate when the app relaunches after crashing during an active workout session.

