

- UIKit
- UIColor
-  init(named:inBundle:compatibleWithTraitCollection:) 

Initializer

# init(named:inBundle:compatibleWithTraitCollection:)

Creates a color object using the named asset that’s compatible with the specified trait collection.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
init?(
    named name: String,
    inBundle bundle: Bundle?,
    compatibleWithTraitCollection traitCollection: UITraitCollection?
)
```

``` source
init?(
    named name: String,
    in bundle: Bundle?,
    compatibleWith traitCollection: UITraitCollection?
)
```

## Parameters 

`name`  

The name of the asset containing the color.

`bundle`  

The bundle containing the asset.

`traitCollection`  

The trait collection that specifies the gamut to use when selecting the color.

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

init?(named: String)

Creates a color object using the information from the named asset.

