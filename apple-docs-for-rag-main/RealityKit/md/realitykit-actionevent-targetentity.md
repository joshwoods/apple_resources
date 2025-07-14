

- RealityKit
- ActionEvent
-  targetEntity 

Instance Property

# targetEntity

The entity the bind target references.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
let targetEntity: Entity?
```

## Discussion

For example, if a bind target references an entity’s transform (i.e. `.transform`), this value is set to that entity.

This may differ from the entity property in the playback controller if the bind target references an entity other than the entity that the animation was played on.

