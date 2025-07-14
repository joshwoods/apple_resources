

- UIKit
-  UIPointerEffect 

Enumeration

# UIPointerEffect

An effect that alters a view’s appearance when a pointer enters the current region.

iOS 13.4+iPadOS 13.4+Mac CatalystvisionOS

``` source
enum UIPointerEffect
```

## Overview

`UIPointerEffect` automatically attempts to determine the appropriate effect for the given preview. Use one of its enumeration cases to request a specific system-provided effect.

## Topics

### Accessing the preview

var preview: UITargetedPreview

A preview of the view used during an interaction’s animations.

### Creating a default effect

case automatic(UITargetedPreview)

A pointer content effect with the given preview’s view.

### Creating a specific effect

case highlight(UITargetedPreview)

An effect where the pointer slides under the given view and morphs into the view’s shape.

case hover(UITargetedPreview, preferredTintMode: UIPointerEffect.TintMode, prefersShadow: Bool, prefersScaledContent: Bool)

An effect where visual changes apply to the view and the pointer retains its default shape.

case lift(UITargetedPreview)

An effect where the pointer slides under the given view and disappears as the view scales up and gains a shadow.

### Enumerations

enum TintMode

An effect that defines how to apply a tint to a view during a pointer interaction.

## Relationships

### Conforms To

- Copyable
- Equatable
- Sendable
- UIHoverEffect

## See Also

### Pointer styles

class UIPointerStyle

An object that defines the pointer shape and effect.

enum UIPointerShape

An object that defines the shape of custom pointers.

class UIPointerAccessory

Constants that describe accessories to display alongside the primary pointer.

