

- HealthKit
- HKWorkoutSession
-  delegate 

Instance Property

# delegate

The workout session’s delegate.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 2.0+

``` source
weak var delegate: (any HKWorkoutSessionDelegate)? { get set }
```

## Discussion

The delegate receives notifications when a workout session’s state changes or when a workout session fails.

## See Also

### Monitoring the session

protocol HKWorkoutSessionDelegate

The session delegate protocol that defines an interface for receiving notifications about errors and changes in the workout session’s state.

