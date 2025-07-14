

- RealityKit
- IKComponent
- IKComponent.Solver
-  maxIterations 

Instance Property

# maxIterations

The maximum number of iterations the solver is allowed to do per frame.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var maxIterations: Int { get set }
```

## Discussion

If the pose satisfies all of the demands using less iterations, the solve stops early.

The initial value is from the respective maxIterations.

Note

Values of `0` or less, result in the constant output of the last solved pose.

