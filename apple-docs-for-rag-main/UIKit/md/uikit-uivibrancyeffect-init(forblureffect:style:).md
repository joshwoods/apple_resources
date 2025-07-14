

- UIKit
- UIVibrancyEffect
-  init(forBlurEffect:style:) 

Initializer

# init(forBlurEffect:style:)

Creates a vibrancy effect with the specified blur and style values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(
    forBlurEffect blurEffect: UIBlurEffect,
    style: UIVibrancyEffectStyle
)
```

``` source
@MainActor
init(
    blurEffect: UIBlurEffect,
    style: UIVibrancyEffectStyle
)
```

## Parameters 

`blurEffect`  

The UIBlurEffect used by the blurred view the vibrancy effect is attached to.

`style`  

The style that defines what level of vibrancy to apply to the content. For a list of possible values, see UIVibrancyEffectStyle.

## Return Value

The vibrancy effect object to use in your visual effect view.

## Discussion

When you create a new vibrancy effect, use the same UIBlurEffect that you used to create the blur view. Using a different UIBlurEffect can cause unwanted visual effect combinations.

## See Also

### Creating a vibrancy effect

init(blurEffect: UIBlurEffect)

Creates a vibrancy effect for a specific blur effect.

enum UIVibrancyEffectStyle

Constants for the vibrancy styles.

