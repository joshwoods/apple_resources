

- RealityKit
- BindPath
- BindPath.Part
-  BindPath.Part.entity(\_:) 

Case

# BindPath.Part.entity(\_:)

A path component for a nested entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
case entity(String)
```

## Discussion

This path component indicates that another component follows, which either contains or identifies the property of the entity that animates.

## See Also

### Choosing the path component

case anchorEntity(String)

A path component for the scene’s anchor entity.

case jointTransforms

A path component to animate joint transforms.

case parameter(String)

A path component to animate a named parameter.

case scene(String)

A path component for a nested scene.

case transform

A path component to animate a transform.

