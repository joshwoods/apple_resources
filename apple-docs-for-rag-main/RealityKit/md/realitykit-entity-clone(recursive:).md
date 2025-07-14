

- RealityKit
- Entity
-  clone(recursive:) 

Instance Method

# clone(recursive:)

Duplicates an entity to create a new entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func clone(recursive: Bool) -> Self
```

## Parameters 

`recursive`  

A Boolean that you set to `true` to recursively copy all the children of the entity. Otherwise, no descendants are copied.

## Return Value

The duplicate.

## Mentioned in 

Manipulating Reality Composer scenes from code

## Discussion

All component data is cloned automatically. If you clone an entity that stores custom data that’s not part of a component, override the didClone(from:) method to copy that data manually.

## See Also

### Creating an entity

init()

Creates a new entity.

convenience init&lt;each T>(components: repeat each T)

Creates an entity with one or multiple components.

convenience init(components: [any Component])

Creates an entity with multiple components.

func didClone(from: Entity)

Tells a newly cloned entity that cloning is complete.

