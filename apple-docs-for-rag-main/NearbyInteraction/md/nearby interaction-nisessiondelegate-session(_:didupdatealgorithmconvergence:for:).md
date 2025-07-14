

- Nearby Interaction
- NISessionDelegate
-  session(\_:didUpdateAlgorithmConvergence:for:) 

Instance Method

# session(\_:didUpdateAlgorithmConvergence:for:)

Provides recommended actions the user can take to facilitate the framework’s Camera Assistance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+watchOS 9.0+

``` source
optional func session(
    _ session: NISession,
    didUpdateAlgorithmConvergence convergence: NIAlgorithmConvergence,
    for object: NINearbyObject?
)
```

## Parameters 

`session`  

The session for which the app leverages Camera Assistance.

`convergence`  

The framework’s state and user recommendations for Camera Assistance.

`object`  

The peer device or third-party accessory. If `nil`, the status refers to the session.

## Discussion

The framework invokes this callback when isCameraAssistanceEnabled is `true` to notify the app of the current convergence state and user-coaching recommendations.

## See Also

### Coaching the user

enum NIAlgorithmConvergenceStatus

The possible states of Camera Assistance.

struct Reason

The possible reasons for the Camera Assistance status.

