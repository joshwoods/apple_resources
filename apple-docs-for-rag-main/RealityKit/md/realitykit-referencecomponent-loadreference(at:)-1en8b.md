

- RealityKit
- ReferenceComponent
-  loadReference(at:) 

Type Method

# loadReference(at:)

Asynchronously loads another entity file that an entity depends on.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
static func loadReference(at entity: Entity) async throws
```

## Parameters 

`entity`  

The entity that holds the ReferenceComponent to load.

