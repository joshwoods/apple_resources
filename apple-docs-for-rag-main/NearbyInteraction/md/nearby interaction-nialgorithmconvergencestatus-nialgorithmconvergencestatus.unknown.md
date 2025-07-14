

- Nearby Interaction
- NIAlgorithmConvergenceStatus
-  NIAlgorithmConvergenceStatus.unknown 

Case

# NIAlgorithmConvergenceStatus.unknown

An indication that the framework is unsure of the Camera Assistance status.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+watchOS 9.0+

``` source
case unknown
```

## Discussion

Look to a subsequent call to session(_:didUpdateAlgorithmConvergence:for:) and check for a more definitive algorithm-convergence status.

## See Also

### Interpreting the convergence state

case converged

A status that indicates the framework’s Camera Assistance feature is operational.

case notConverged([NIAlgorithmConvergenceStatus.Reason])

A status that indicates the framework’s Camera Assistance feature requires action from the user.

