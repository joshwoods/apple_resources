

- RealityKit
- IKComponent
-  resource 

Instance Property

# resource

Reference to the resource describing the desired inverse kinematics setup.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var resource: IKResource?
```

## Discussion

Note

There is one engine tick delay between setting new resource and the change reflected in `solvers`.

