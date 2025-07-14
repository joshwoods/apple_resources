

- GameplayKit
- GKComponentSystem
-  addComponent(foundIn:) 

Instance Method

# addComponent(foundIn:)

Adds any instances of the component system’s component class in the specified entity to the component system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func addComponent(foundIn entity: GKEntity)
```

## Parameters 

`entity`  

An entity.

## Discussion

This method examines the components array of the specified entity, adding any components whose type matches the component system’s componentClass property to the component system.

## See Also

### Managing a List of Components

var componentClass: AnyClass

The class of components managed by the component system.

var components: [ComponentType]

The component system’s list of components.

func addComponent(ComponentType)

Adds a component instance to the component system.

func removeComponent(ComponentType)

Removes the specified component instance from the component system.

func removeComponent(foundIn: GKEntity)

Removes any instances of the component system’s component class in the specified entity from the component system.

