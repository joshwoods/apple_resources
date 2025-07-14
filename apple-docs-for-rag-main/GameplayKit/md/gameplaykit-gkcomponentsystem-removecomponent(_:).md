

- GameplayKit
- GKComponentSystem
-  removeComponent(\_:) 

Instance Method

# removeComponent(\_:)

Removes the specified component instance from the component system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func removeComponent(_ component: ComponentType)
```

## Parameters 

`component`  

An instance of a GKComponent subclass in the component system.

## Discussion

If the specified component is not in the component system, this method has no effect.

## See Also

### Managing a List of Components

var componentClass: AnyClass

The class of components managed by the component system.

var components: [ComponentType]

The component system’s list of components.

func addComponent(ComponentType)

Adds a component instance to the component system.

func addComponent(foundIn: GKEntity)

Adds any instances of the component system’s component class in the specified entity to the component system.

func removeComponent(foundIn: GKEntity)

Removes any instances of the component system’s component class in the specified entity from the component system.

