

- AppKit
- NSColorSpace
-  availableColorSpaces(with:) 

Type Method

# availableColorSpaces(with:)

Returns the list of color spaces available on the system that are displayed in the color panel, in the order they are displayed in the color panel.

macOS 10.6+

``` source
class func availableColorSpaces(with model: NSColorSpace.Model) -> [NSColorSpace]
```

## Parameters 

`model`  

The model to return the color spaces for.

## Return Value

The list of color spaces, or an empty array if no color spaces are available for the specified model.

## Discussion

This method doesn’t return color spaces created on the fly or spaces without user-displayable names. Pass NSUnknownColorSpaceModel as `model` to get all available color spaces.

