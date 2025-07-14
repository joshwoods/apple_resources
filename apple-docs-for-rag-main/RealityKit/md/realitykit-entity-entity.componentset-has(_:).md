

- RealityKit
- Entity
- Entity.ComponentSet
-  has(\_:) 

Instance Method

# has(\_:)

Returns a Boolean value that indicates whether the set contains a component of the given type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func has(_ componentType: any Component.Type) -> Bool
```

## Parameters 

`componentType`  

A component type, like `ModelComponent.Self`.

## Return Value

A Boolean value that’s `true` if the set contains a component of the given type.

