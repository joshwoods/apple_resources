

- UIKit
-  UIHoverEffect 

Protocol

# UIHoverEffect

A hover effect that can apply to a view through a hover style.

iOS 17.0+iPadOS 17.0+Mac CatalystvisionOS 1.0+

``` source
protocol UIHoverEffect
```

## Overview

You don’t conform to this protocol directly. Instead, you use a built-in UIHoverEffect like UIHoverAutomaticEffect.

## Topics

### Choosing a hover effect

static var automatic: UIHoverAutomaticEffect

A system-default hover effect that automatically selects the appropriate effect based on the view to which it applies.

static var highlight: UIHoverHighlightEffect

An effect that applies a highlight to the view on hover.

static var lift: UIHoverLiftEffect

An effect that can visually lift the view on hover where appropriate.

## Relationships

### Conforming Types

- UIHoverAutomaticEffect
- UIHoverHighlightEffect
- UIHoverLiftEffect
- UIPointerEffect

## See Also

### Specifying a hover effect

var effect: any UIHoverEffect

The effect to apply to the view with this style.

struct UIHoverAutomaticEffect

A system-default hover effect that automatically selects the appropriate effect based on the view to which it applies.

struct UIHoverHighlightEffect

An effect that applies a highlight to the view on hover.

struct UIHoverLiftEffect

An effect that can visually lift the view on hover where appropriate.

