

- External Accessory
- EAAccessoryManager
-  connectedAccessories 

Instance Property

# connectedAccessories

The accessory objects corresponding to the list of currently connected accessories.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
var connectedAccessories: [EAAccessory] { get }
```

## Discussion

This property contains an array of EAAccessory objects. Each object corresponds to an accessory that is connected and available for your application to use. Because the contents of this property can change dynamically based on the connection and disconnection of accessories, you should not cache the value of this property.

