

- HomeKit
- HMAccessory
-  category 

Instance Property

# category

The category to which the accessory belongs.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var category: HMAccessoryCategory { get }
```

## Discussion

The accessory’s category property contains an instance of the HMAccessoryCategory class that indicates the kind of accessory, like light bulb, garage door opener, or faucet. Use this information to help users distinguish among different accessories in their environment.

## See Also

### Categorizing an accessory

class HMAccessoryCategory

A category for a HomeKit accessory.

