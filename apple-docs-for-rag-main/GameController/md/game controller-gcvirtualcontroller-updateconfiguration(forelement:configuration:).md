

- Game Controller
- GCVirtualController
-  updateConfiguration(forElement:configuration:) 

Instance Method

# updateConfiguration(forElement:configuration:)

Changes the configuration for one of the virtual controller’s input elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func updateConfiguration(
    forElement element: String,
    configuration config: (GCVirtualController.ElementConfiguration) -> GCVirtualController.ElementConfiguration
)
```

## Parameters 

`element`  

The element whose configuration you want to change. For the possible values of this parameter, see the elements property.

`config`  

The new configuration for the element.

## Mentioned in 

Adding touch controls to games that support game controllers in iOS

## See Also

### Customizing the elements

class ElementConfiguration

The properties of a virtual controller’s element that you can customize.

