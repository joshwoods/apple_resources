

- WatchKit
- WKExtensionDelegate
-  handleActiveWorkoutRecovery() 

Instance Method

# handleActiveWorkoutRecovery()

Tells the delegate when the app relaunches after crashing during an active workout session.

watchOS 5.0+

``` source
@MainActor
optional func handleActiveWorkoutRecovery()
```

## Discussion

To recover from a crash, call your HealthKit store’s recoverActiveWorkoutSession(completion:) method to receive a new workout session. You can then set up your data source and delegate as described in Running workout sessions.

## See Also

### Related Documentation

func recoverActiveWorkoutSession(completion: (HKWorkoutSession?, (any Error)?) -> Void)

Recovers an active workout session.

### Handling a workout session

func handle(HKWorkoutConfiguration)

Tells the delegate that the user started a workout session on the paired iPhone.

