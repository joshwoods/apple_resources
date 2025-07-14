

- ARKit
- ARReferenceImage
-  name 

Instance Property

# name

A descriptive name for the image.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.1+

``` source
var name: String? { get set }
```

## Discussion

For reference images loaded from an Xcode asset catalog, this property is the name assigned in the asset catalog. For programmatically created reference images, this value is `nil`.

Note

This string is not localized text intended for user display. However, in debugging you can use this property to indicate which image was detected.

## See Also

### Examining a Reference Image

var physicalSize: CGSize

The real-world dimensions, in meters, of the image.

var resourceGroupName: String?

The AR resource group name for this image.

