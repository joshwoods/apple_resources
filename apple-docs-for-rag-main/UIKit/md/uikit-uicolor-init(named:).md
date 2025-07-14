

- UIKit
- UIColor
-  init(named:) 

Initializer

# init(named:)

Creates a color object using the information from the named asset.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init?(named name: String)
```

## Parameters 

`name`  

The name of the asset containing the color.

## Return Value

An initialized color object. The returned object uses the color space specified for the asset.

## See Also

### Creating a color from component values

init(white: CGFloat, alpha: CGFloat)

Creates a color object using the specified opacity and grayscale values.

init(hue: CGFloat, saturation: CGFloat, brightness: CGFloat, alpha: CGFloat)

Creates a color object using the specified opacity and HSB color space component values.

init(red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object using the specified opacity and RGB component values.

init(displayP3Red: CGFloat, green: CGFloat, blue: CGFloat, alpha: CGFloat)

Creates a color object using the specified opacity and RGB component values in the Display P3 color space.

init?(named: String, inBundle: Bundle?, compatibleWithTraitCollection: UITraitCollection?)

Creates a color object using the named asset that’s compatible with the specified trait collection.

