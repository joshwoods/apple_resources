

- RealityKit
- System
-  init(scene:) 

Initializer

# init(scene:)

Creates a new system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
init(scene: Scene)
```

**Required**

## Parameters 

`scene`  

The scene this system affects.

## Mentioned in 

Implementing systems for entities in a scene

## Discussion

There’s no need to instantiate your own systems, so don’t call this method. Instead, register your system with RealityKit by calling registerSystem(). RealityKit automatically creates an instance of every registered system for every scene.

