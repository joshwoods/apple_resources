

- Nearby Interaction
- NIAlgorithmConvergenceStatus
-  NIAlgorithmConvergenceStatus.converged 

Case

# NIAlgorithmConvergenceStatus.converged

A status that indicates the framework’s Camera Assistance feature is operational.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+watchOS 9.0+

``` source
case converged
```

## Discussion

In this state, the app doesn’t need to coach the user and receives all the benefits of Camera Assistance described in isCameraAssistanceEnabled.

## See Also

### Interpreting the convergence state

case notConverged([NIAlgorithmConvergenceStatus.Reason])

A status that indicates the framework’s Camera Assistance feature requires action from the user.

case unknown

An indication that the framework is unsure of the Camera Assistance status.

