

- AppKit
- NSViewAnimation
-  viewAnimations 

Instance Property

# viewAnimations

The dictionaries defining the objects to animate.

macOS

``` source
var viewAnimations: [[NSViewAnimation.Key : Any]] { get set }
```

## See Also

### Getting and setting view-animation dictionaries

struct Key

The following string constants are keys for the dictionaries in the array passed into init(viewAnimations:) and viewAnimations.

struct EffectName

The following constants specify the animation effect to apply and are used as values for the animation effect property of the animation view. See the description of effect for usage details.

