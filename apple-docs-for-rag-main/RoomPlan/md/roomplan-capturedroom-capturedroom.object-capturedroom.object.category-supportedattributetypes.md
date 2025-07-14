

- RoomPlan
- CapturedRoom
- CapturedRoom.Object
- CapturedRoom.Object.Category
-  supportedAttributeTypes 

Instance Property

# supportedAttributeTypes

Defines the attributes types compatible with a particular object category.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
var supportedAttributeTypes: [any CapturedRoomAttribute.Type] { get }
```

## Discussion

The framework defines the contents of this array. Only compatible attributes can pair up in association with a 3D model, for example, with the CapturedRoom.ModelProvider function setModelFileURL(_:for:). These CapturedRoom.ModelProvider functions for `setModelFileURL` and `modelFileURL` throw CapturedRoom.ModelProvider.Error.attributeCombinationNotSupported if no object category supports all of the attributes in the arguments to their call.

## See Also

### Determining supported attributes

var supportedCombinations: [[any CapturedRoomAttribute]]

An array of supported attributes that differs by category.

func supportsCombination([any CapturedRoomAttribute]) -> Bool

Returns a Boolean value that indicates whether a category supports the given attribute combination.

