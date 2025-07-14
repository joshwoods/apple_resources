

- Nearby Interaction
- NIAlgorithmConvergenceStatus
-  NIAlgorithmConvergenceStatus.notConverged(\_:) 

Case

# NIAlgorithmConvergenceStatus.notConverged(\_:)

A status that indicates the framework’s Camera Assistance feature requires action from the user.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+watchOS 9.0+

``` source
case notConverged([NIAlgorithmConvergenceStatus.Reason])
```

## Parameters 

`reason`  

A user action that the framework recommends to get the Camera Assistance feature operational.

## Discussion

In this state, the framework needs more information about the user’s physical environment before setting horizontalAngle and/or verticalDirectionEstimate.

Look to the reasons array of the `convergence` object provided by session(_:didUpdateAlgorithmConvergence:for:) for more information on the cause. Each reason indicates a specific action the user can do to provide ARKit with the necessary camera data to support Nearby Interaction’s Camera Assistance.

## See Also

### Interpreting the convergence state

case converged

A status that indicates the framework’s Camera Assistance feature is operational.

case unknown

An indication that the framework is unsure of the Camera Assistance status.

