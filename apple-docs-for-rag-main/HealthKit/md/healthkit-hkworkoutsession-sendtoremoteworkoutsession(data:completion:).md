

- HealthKit
- HKWorkoutSession
-  sendToRemoteWorkoutSession(data:completion:) 

Instance Method

# sendToRemoteWorkoutSession(data:completion:)

Sends the provided data to the remote workout session.

iOS 17.0+iPadOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func sendToRemoteWorkoutSession(
    data: Data,
    completion: @escaping (Bool, (any Error)?) -> Void
)
```

``` source
func sendToRemoteWorkoutSession(data: Data) async throws
```

## Parameters 

`data`  

A data object that contains the data your app is sending to the remote workout session.

`completion`  

A block that the system calls when the send attempt is complete. The system passes the following parameters:

`success`  
A Boolean value that indicates whether the system successfully sent the data.

`error`  
If `sucess` is false, this contains an object that describes the error. Otherwise, it’s `nil`.

## Discussion

Call this method to send data to your remote workout session. You can send data from either the HKWorkoutSessionType.mirrored or HKWorkoutSessionType.primary session.

```
let archivedData = try? NSKeyedArchiver.archivedData(withRootObject: data, requiringSecureCoding: true)
guard let archivedData = archivedData, !archivedData.isEmpty else {
    // Handle the error here.
    fatalError("*** Encoded data is empty ***")
}

// Send the data to the companion iPhone.
Task {
    do {
        try await session.sendToRemoteWorkoutSession(data: archivedData)
    }
    catch {
        // Handle the error here.
        fatalError("*** An error occurred while sending the health data to the companion iPhone: \(error.localizedDescription) ***")
    }
}
```

## See Also

### Working with remote workout sessions

func startMirroringToCompanionDevice(completion: (Bool, (any Error)?) -> Void)

Starts mirroring the workout session to the companion iOS device.

func stopMirroringToCompanionDevice(completion: (Bool, (any Error)?) -> Void)

Stops mirroring the workout session to the companion iOS device.

