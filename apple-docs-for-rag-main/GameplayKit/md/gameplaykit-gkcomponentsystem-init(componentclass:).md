

- GameplayKit
- GKComponentSystem
-  init(componentClass:) 

Initializer

# init(componentClass:)

Initializes a component system to manage components of the specified class.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(componentClass cls: AnyClass)
```

## Return Value

A new component system.

## Discussion

Each GKComponentSystem object manages components of a specific GKComponent subclass, which you specify with the `class` parameter in this intializer. After initializing a component system, you may add components to it only if their type matches the system’s component class.

For more information, see GameplayKit Programming Guide.

