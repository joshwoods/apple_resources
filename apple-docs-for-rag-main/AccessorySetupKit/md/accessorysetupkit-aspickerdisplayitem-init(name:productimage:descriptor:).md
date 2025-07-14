

- AccessorySetupKit
- ASPickerDisplayItem
-  init(name:productImage:descriptor:) 

Initializer

# init(name:productImage:descriptor:)

Creates a picker display item with a name and image to display and a descriptor to match discovered accessories.

iOS 18.0+iPadOS 18.0+

``` source
init(
    name: String,
    productImage: UIImage,
    descriptor: ASDiscoveryDescriptor
)
```

## Parameters 

`name`  

The accessory name to display in the picker.

`productImage`  

An image of the accessory to display in the picker.

`descriptor`  

A descriptor that the picker uses to determine which discovered accessories to display.

