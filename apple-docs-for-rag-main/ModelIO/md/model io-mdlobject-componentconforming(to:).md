

- Model I/O
- MDLObject
-  componentConforming(to:) 

Instance Method

# componentConforming(to:)

Returns the object’s component for the specified protocol.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func componentConforming(to protocol: Protocol) -> (any MDLComponent)?
```

## Parameters 

`protocol`  

The protocol for which to retrieve a component. This protocol must extend the MDLComponent protocol.

## Return Value

The object’s component for the protocol, or `nil` if the object does not have such a component.

## Discussion

Components are the basis for customizable file format and object graph support in Model I/O. By default, the MDLObject uses the MDLObjectContainerComponent and MDLTransformComponent protocols to model object hierarchies and spatial transforms: When you load an object graph from a MDLAsset instance, Model I/O creates container and transforms components to represent the object hierarchy and spatial relationships described in the asset file. However, you can also create custom components. For example, a custom component protocol could add support for an asset format that encodes gameplay-related information such as scripting triggers, or a custom class for the MDLObjectContainerComponent could implement other ways to store or traverse object hierarchies.

## See Also

### Customizing Objects with Components

func setComponent(any MDLComponent, for: Protocol)

Associates a component with the object for the specified protocol.

