

- ARKit
- ARReferenceImage
-  resourceGroupName 

Instance Property

# resourceGroupName

The AR resource group name for this image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var resourceGroupName: String? { get }
```

## Discussion

If ARKit loaded this image from an AR resource group in an asset catalog, ARKit sets the value of this property to the resource group’s name. Otherwise, the value of this property is `nil`\>.

## See Also

### Examining a Reference Image

var name: String?

A descriptive name for the image.

var physicalSize: CGSize

The real-world dimensions, in meters, of the image.

