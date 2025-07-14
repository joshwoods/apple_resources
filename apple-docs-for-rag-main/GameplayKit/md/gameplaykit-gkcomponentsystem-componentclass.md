

- GameplayKit
- GKComponentSystem
-  componentClass 

Instance Property

# componentClass

The class of components managed by the component system.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var componentClass: AnyClass { get }
```

## Discussion

Each GKComponentSystem object manages components of a specific GKComponent subclass. You specify the component class to be used by a system when creating it with the init(componentClass:) initializer. Afterward, you may add components to the system only if their type matches the system’s component class.

## See Also

### Managing a List of Components

var components: [ComponentType]

The component system’s list of components.

func addComponent(ComponentType)

Adds a component instance to the component system.

func addComponent(foundIn: GKEntity)

Adds any instances of the component system’s component class in the specified entity to the component system.

func removeComponent(ComponentType)

Removes the specified component instance from the component system.

func removeComponent(foundIn: GKEntity)

Removes any instances of the component system’s component class in the specified entity from the component system.

