

- SwiftUI
-  AutomaticHoverEffect 

Structure

# AutomaticHoverEffect

The default hover effect based on the surrounding context.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
struct AutomaticHoverEffect
```

## Overview

The automatic effect will resolve to any defaultHoverEffect(_:) applied to the current View hierarchy, or a system-defined effect if no default effect has been defined.

You can also use automatic to construct this hover effect.

## Topics

### Initializers

init()

Creates an automatic hover effect.

## Relationships

### Conforms To

- CustomHoverEffect

## See Also

### Supporting types

struct EmptyHoverEffect

A base hover effect used to build additional effects.

struct HighlightHoverEffect

A hover effect that highlights views using a light source to indicate position.

struct LiftHoverEffect

A hover effect that slides the pointer under the view and disappears as the view scales up and gains a shadow.

