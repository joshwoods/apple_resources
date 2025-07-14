

- HealthKit
- HKWorkoutSessionDelegate
-  workoutSession(\_:didDisconnectFromRemoteDeviceWithError:) 

Instance Method

# workoutSession(\_:didDisconnectFromRemoteDeviceWithError:)

Tells the delegate that the mirrored workout session disconnected from the primary session.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOSvisionOS 1.0+watchOS 10.0+

``` source
optional func workoutSession(
    _ workoutSession: HKWorkoutSession,
    didDisconnectFromRemoteDeviceWithError error: (any Error)?
)
```

## Parameters 

`workoutSession`  

The mirrored workout session that disconnected.

`error`  

If an error caused the disconnection, then this parameter contains the error value. Otherwise, it’s `nil`.

## Discussion

After the system calls this method, the provided workout session is no longer valid, and you can no longer use it.

```
func clearWorkoutSession() {
    state = .notRunning
    session = nil
}

nonisolated func workoutSession(_ workoutSession: HKWorkoutSession, didDisconnectFromRemoteDeviceWithError error: Error?) {
    Task {
        // Clear the old session.
        await clearWorkoutSession()
    }

    logger.debug("*** Remote workout session disconnected. ***")
    if let error {
        fatalError("*** Disconnected with an error: \(error.localizedDescription) ***")
    }
}
```

If the primary workout session is still running, it automatically tries to reconnect. If successful, the companion iOS device calls the workoutSessionMirroringStartHandler block again, passing in a new, valid HKWorkoutSession instance.

## See Also

### Working with mirrored sessions

func workoutSession(HKWorkoutSession, didReceiveDataFromRemoteWorkoutSession: [Data])

Passes data from the remote workout session to the session delegate.

