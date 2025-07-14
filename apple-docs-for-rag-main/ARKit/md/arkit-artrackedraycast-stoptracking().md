

- ARKit
- ARTrackedRaycast
-  stopTracking() 

Instance Method

# stopTracking()

Stops repeating the raycast query.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
func stopTracking()
```

## Discussion

A tracked raycast updates continuously until you stop it explicitly by calling stopTracking(). A raycast will automatically stop when:

- ARKit calls sessionWasInterrupted(_:).

- You change the session’s configuration.

- You deallocate the ARTrackedRaycast.

