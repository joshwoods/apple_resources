

- RealityKit
- BindTarget
-  BindTarget.path(\_:) 

Case

# BindTarget.path(\_:)

Provides a complex bind path capable of animating additional entities other than the current entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case path(BindPath)
```

## See Also

### Choosing a bind target

case `internal`(InternalBindPath)

A bind target that refers to a framework-provided property.

case jointTransforms

An option that specifies that the entity’s joint transforms animate.

case parameter(String)

Provides a property that animates from the given textual name.

case transform

A option that specifies that the target entity’s transform animates.

