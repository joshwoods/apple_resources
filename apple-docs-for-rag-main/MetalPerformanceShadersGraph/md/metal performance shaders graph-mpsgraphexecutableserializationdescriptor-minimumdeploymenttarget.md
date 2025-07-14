

- Metal Performance Shaders Graph
- MPSGraphExecutableSerializationDescriptor
-  minimumDeploymentTarget 

Instance Property

# minimumDeploymentTarget

The minimum deployment target to serialize the executable.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var minimumDeploymentTarget: String { get set }
```

## Discussion

If not set, the package created will target the latest version of the `deploymentPlatform` set.

