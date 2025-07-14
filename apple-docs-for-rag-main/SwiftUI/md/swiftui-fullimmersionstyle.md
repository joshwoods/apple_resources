

- SwiftUI
-  FullImmersionStyle 

Structure

# FullImmersionStyle

An immersion style that displays unbounded content that completely replaces passthrough video.

visionOS 1.0+

``` source
struct FullImmersionStyle
```

## Overview

When this immersion style is selected, the immersion amount reported by the closure of `View/onImmersionChange(_:)` is `1.0`.

Use full with the immersionStyle(selection:in:)modifier to specify this style.

## Topics

### Creating the immersion style

init()

## Relationships

### Conforms To

- ImmersionStyle

## See Also

### Supporting types

struct AutomaticImmersionStyle

The default style of immersive spaces.

struct MixedImmersionStyle

An immersion style that displays unbounded content intermixed with other app content, along with passthrough video.

struct ProgressiveImmersionStyle

An immersion style that displays unbounded content that partially replaces passthrough video.

