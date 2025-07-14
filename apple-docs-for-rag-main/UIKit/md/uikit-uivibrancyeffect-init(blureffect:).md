

- UIKit
- UIVibrancyEffect
-  init(blurEffect:) 

Initializer

# init(blurEffect:)

Creates a vibrancy effect for a specific blur effect.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
init(blurEffect: UIBlurEffect)
```

## Parameters 

`blurEffect`  

The UIBlurEffect used by the blurred view the vibrancy effect is attached to.

## Return Value

The vibrancy effect to be used by a UIVisualEffectView object.

## Discussion

When you create a new vibrancy effect, use the same UIBlurEffect that you used to create the blur view. Using a different UIBlurEffect can cause unwanted visual effect combinations.

## See Also

### Creating a vibrancy effect

init(forBlurEffect: UIBlurEffect, style: UIVibrancyEffectStyle)

Creates a vibrancy effect with the specified blur and style values.

enum UIVibrancyEffectStyle

Constants for the vibrancy styles.

