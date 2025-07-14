

- GameplayKit
- GKComponent
-  willRemoveFromEntity() 

Instance Method

# willRemoveFromEntity()

Notifies the component that it has been removed from an entity.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func willRemoveFromEntity()
```

## Discussion

Override this method in a component subclass if you need to perform game logic when the component is removed from to an entity. For example, if one component’s behavior depends on the presence of other components in the same entity, you can examine the entity’s components array in this method and take action accordingly.

## See Also

### Working with Entities

var entity: GKEntity?

The entity that owns this component.

func didAddToEntity()

Notifies the component that it has been assigned to an entity.

