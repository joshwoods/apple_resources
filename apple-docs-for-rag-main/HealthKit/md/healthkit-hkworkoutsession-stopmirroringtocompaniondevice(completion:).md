

- HealthKit
- HKWorkoutSession
-  stopMirroringToCompanionDevice(completion:) 

Instance Method

# stopMirroringToCompanionDevice(completion:)

Stops mirroring the workout session to the companion iOS device.

watchOS 10.0+

``` source
func stopMirroringToCompanionDevice(completion: @escaping (Bool, (any Error)?) -> Void)
```

``` source
func stopMirroringToCompanionDevice() async throws
```

## Parameters 

`completion`  

A block that the system calls when the stop request is complete. The system sets the following parameters:

`success`  
A Boolean value that indicates whether the system successfully stopped mirroring the session.

`error`  
If `success` is false, this contains an object that describes the error. Otherwise, it’s `nil`.

## Discussion

Call this method in your watchOS app to stop the mirrored workout session on the companion iOS app. After the mirroring stops, the system calls the workoutSession(_:didDisconnectFromRemoteDeviceWithError:) method on the iOS companion’s session delegate.

```
session.end()

// Stop the workout builder and save the workout data.
do {
    try await builder.endCollection(at: Date())
    try await builder.finishWorkout()
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while stoping the workout: \(error.localizedDescription) ***")
}

// Stop the mirrored workout on the iOS companion.
do {
    try await session.stopMirroringToCompanionDevice()
} catch {
    // Handle the error here.
    fatalError("*** An error occurred while stoping the mirrored workout: \(error.localizedDescription) ***")
}
```

## See Also

### Working with remote workout sessions

func startMirroringToCompanionDevice(completion: (Bool, (any Error)?) -> Void)

Starts mirroring the workout session to the companion iOS device.

func sendToRemoteWorkoutSession(data: Data, completion: (Bool, (any Error)?) -> Void)

Sends the provided data to the remote workout session.

