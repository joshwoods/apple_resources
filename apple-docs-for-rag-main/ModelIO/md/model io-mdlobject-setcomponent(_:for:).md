

- Model I/O
- MDLObject
-  setComponent(\_:for:) 

Instance Method

# setComponent(\_:for:)

Associates a component with the object for the specified protocol.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func setComponent(
    _ component: any MDLComponent,
    for protocol: Protocol
)
```

## Parameters 

`component`  

The component to associate with the object. The component class must adopt the protocol specified in the `protocol` parameter.

`protocol`  

The protocol whose functionality the component provides.

## Discussion

Components are the basis for customizable file format and object graph support in Model I/O. By default, the MDLObject uses the MDLObjectContainerComponent and MDLTransformComponent protocols to model object hierarchies and spatial transforms: When you load an object graph from a MDLAsset instance, Model I/O creates container and transforms components to represent the object hierarchy and spatial relationships described in the asset file. However, you can also create custom components. For example, a custom component protocol could add support for an asset format that encodes gameplay-related information such as scripting triggers, or a custom class for the MDLObjectContainerComponent could implement other ways to store or traverse object hierarchies.

## See Also

### Customizing Objects with Components

func componentConforming(to: Protocol) -> (any MDLComponent)?

Returns the object’s component for the specified protocol.

