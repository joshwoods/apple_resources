

- RealityKit
- System
-  registerSystem() 

Type Method

# registerSystem()

Registers a system with RealityKit.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
@MainActor @preconcurrency
static func registerSystem()
```

## Mentioned in 

Implementing systems for entities in a scene

## Discussion

Calling this method informs RealityKit of a system of defined behavior for its scenes. RealityKit automatically creates an instance of all registered systems for every scene and calls every registered system’s update(context:) method on every scene update.

If you call registerSystem() multiple times, RealityKit ignores additional calls after the first.

