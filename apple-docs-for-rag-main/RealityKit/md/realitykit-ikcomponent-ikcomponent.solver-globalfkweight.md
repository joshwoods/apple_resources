

- RealityKit
- IKComponent
- IKComponent.Solver
-  globalFkWeight 

Instance Property

# globalFkWeight

The solver global forward kinematics demand’s weight.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var globalFkWeight: Float { get set }
```

## Discussion

Multiplied with the per-joint per-axis forward kinematics weight fkWeightPerAxis.

The initial value is from the respective globalFkWeight.

