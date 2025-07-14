

- RealityKit
- BindPath
- BindPath.Part
-  BindPath.Part.scene(\_:) 

Case

# BindPath.Part.scene(\_:)

A path component for a nested scene.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case scene(String)
```

## Discussion

This path component indicates that another component follows, and at the same time specifies the entity, scene, or property that animates.

Because no path contains nested scenes, this component exists only as the first element of a multicomponent path.

## See Also

### Choosing the path component

case anchorEntity(String)

A path component for the scene’s anchor entity.

case entity(String)

A path component for a nested entity.

case jointTransforms

A path component to animate joint transforms.

case parameter(String)

A path component to animate a named parameter.

case transform

A path component to animate a transform.

