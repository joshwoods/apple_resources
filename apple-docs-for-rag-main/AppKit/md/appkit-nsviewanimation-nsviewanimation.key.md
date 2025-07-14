

- AppKit
- NSViewAnimation
-  NSViewAnimation.Key 

Structure

# NSViewAnimation.Key

The following string constants are keys for the dictionaries in the array passed into init(viewAnimations:) and viewAnimations.

macOS

``` source
struct Key
```

## Topics

### Keys

static let effect: NSViewAnimation.Key

An effect to apply to the animation.

static let endFrame: NSViewAnimation.Key

The size and location of the window or view at the end of the animation.

static let startFrame: NSViewAnimation.Key

The size and location of the window or view at the start of the animation.

static let target: NSViewAnimation.Key

The target of the animation.

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

struct EffectName

The following constants specify the animation effect to apply and are used as values for the animation effect property of the animation view. See the description of effect for usage details.

