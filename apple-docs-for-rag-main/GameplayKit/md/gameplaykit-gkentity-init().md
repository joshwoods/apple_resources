

- GameplayKit
- GKEntity
-  init() 

Initializer

# init()

Initializes a new entity object.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init()
```

## Return Value

A new entity object.

## Discussion

If you create a GKEntity subclass and define any additional initializers, you must delegate to this initializer. You do not need to subclass GKEntity to use Entity-Component architecture—generally, you should create a custom entity class only when you need a place to store state or resources that are shared by multiple components.

For more information, see GameplayKit Programming Guide.

