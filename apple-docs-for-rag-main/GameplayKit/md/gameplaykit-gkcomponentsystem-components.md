

- GameplayKit
- GKComponentSystem
-  components 

Instance Property

# components

The component system’s list of components.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var components: [ComponentType] { get }
```

## Discussion

Calling a method of the system’s component class forwards that message to every component in this array.

Important among component-specific messages is the update(deltaTime:) method—call this method on a component system to perform per-frame updates for all the component instances it manages.

## See Also

### Managing a List of Components

var componentClass: AnyClass

The class of components managed by the component system.

func addComponent(ComponentType)

Adds a component instance to the component system.

func addComponent(foundIn: GKEntity)

Adds any instances of the component system’s component class in the specified entity to the component system.

func removeComponent(ComponentType)

Removes the specified component instance from the component system.

func removeComponent(foundIn: GKEntity)

Removes any instances of the component system’s component class in the specified entity from the component system.

