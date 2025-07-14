

- SwiftUI
-  ProgressiveImmersionStyle 

Structure

# ProgressiveImmersionStyle

An immersion style that displays unbounded content that partially replaces passthrough video.

visionOS 1.0+

``` source
struct ProgressiveImmersionStyle
```

## Overview

Use progressive with the immersionStyle(selection:in:)modifier to specify this style.

## Topics

### Creating the immersion style

init()

An immersion style that displays unbounded content that partially replaces passthrough video.

### Initializers

init(immersion:initialAmount:)

An immersion style that displays unbounded content that partially replaces passthrough video.

### Instance Properties

let initialImmersionAmount: Double?

The initial amount of immersion used for this instance of the style.

let maximumImmersionAmount: Double?

The maximum amount of immersion used for this instance of the style.

let minimumImmersionAmount: Double?

The minimum amount of immersion used for this instance of the style.

## Relationships

### Conforms To

- ImmersionStyle

## See Also

### Supporting types

struct AutomaticImmersionStyle

The default style of immersive spaces.

struct FullImmersionStyle

An immersion style that displays unbounded content that completely replaces passthrough video.

struct MixedImmersionStyle

An immersion style that displays unbounded content intermixed with other app content, along with passthrough video.

