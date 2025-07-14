

- GameplayKit
- GKEntity
-  addComponent(\_:) 

Instance Method

# addComponent(\_:)

Adds a component to the entity.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func addComponent(_ component: GKComponent)
```

## Parameters 

`component`  

An instance of a GKComponent subclass.

## Discussion

You create components by subclassing GKEntity to implement reusable behavior. Then, use this method to incorporate the behavior of a component class into that entity.

An entity’s components list never has more than one instance of any component class—if the entity already contains a component of the same class as the `component` parameter, calling this method will replace that component.

## See Also

### Managing an Entity’s List of Components

var components: [GKComponent]

The entity’s list of components.

