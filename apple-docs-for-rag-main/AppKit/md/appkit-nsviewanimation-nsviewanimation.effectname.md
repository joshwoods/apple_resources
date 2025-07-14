

- AppKit
- NSViewAnimation
-  NSViewAnimation.EffectName 

Structure

# NSViewAnimation.EffectName

The following constants specify the animation effect to apply and are used as values for the animation effect property of the animation view. See the description of effect for usage details.

macOS

``` source
struct EffectName
```

## Topics

### Effect Names

static let fadeIn: NSViewAnimation.EffectName

Specifies a fade-in type of effect.

static let fadeOut: NSViewAnimation.EffectName

Specifies a fade-out type of effect.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting and setting view-animation dictionaries

var viewAnimations: [[NSViewAnimation.Key : Any]]

The dictionaries defining the objects to animate.

struct Key

The following string constants are keys for the dictionaries in the array passed into init(viewAnimations:) and viewAnimations.

