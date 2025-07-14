

- RealityKit
- ActionEntityResolution
-  ActionEntityResolution.entityPath(\_:) 

Case

# ActionEntityResolution.entityPath(\_:)

An option that resolves an entity by specifying a bind path relative to the entity playing the action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
case entityPath(BindTarget.EntityPath)
```

## Discussion

Use this to resolve a `BindTarget.EntityPath` from the entity playing the action. The targeted entity will have the action applied to it.

