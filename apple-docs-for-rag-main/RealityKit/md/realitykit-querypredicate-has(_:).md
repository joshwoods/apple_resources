

- RealityKit
- QueryPredicate
-  has(\_:) 

Type Method

# has(\_:)

Creates a new predicate that describes entities that have a specific component.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
static func has(_ t: T.Type) -> QueryPredicate where T : Component
```

## Parameters 

`t`  

The type of component.

## Return Value

A predicate that describes entities with a specified component.

## Discussion

To create a `has` predicate, pass the component class’s `self` property.

```
let myPredicate = QueryPredicate.has(ModelComponent.self)
```

