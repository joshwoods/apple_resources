

- ARKit
- ReferenceImage
-  resourceGroupName 

Instance Property

# resourceGroupName

A string value the represents the name of the resource group the framework loads an image from.

visionOS 2.0+

``` source
var resourceGroupName: String? { get }
```

## Discussion

The property contains a value only if the framework loads a reference image from a resource group. Otherwise, it’s `nil`.

## See Also

### Inspecting a reference image

var physicalSize: CGSize

The size, in meters, of a reference image in the real world.

var name: String?

The name of a reference image.

var description: String

A textual representation of this reference image.

