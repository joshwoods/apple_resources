

- GameplayKit
- GKComponentSystem
-  addComponent(\_:) 

Instance Method

# addComponent(\_:)

Adds a component instance to the component system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func addComponent(_ component: ComponentType)
```

## Parameters 

`component`  

An instance of a GKComponent subclass.

## Discussion

The component instance must be of the same GKComponent subclass specified by the componentClass property.

## See Also

### Managing a List of Components

var componentClass: AnyClass

The class of components managed by the component system.

var components: [ComponentType]

The component system’s list of components.

func addComponent(foundIn: GKEntity)

Adds any instances of the component system’s component class in the specified entity to the component system.

func removeComponent(ComponentType)

Removes the specified component instance from the component system.

func removeComponent(foundIn: GKEntity)

Removes any instances of the component system’s component class in the specified entity from the component system.

