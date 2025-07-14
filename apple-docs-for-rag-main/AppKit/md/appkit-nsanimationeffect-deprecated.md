

- AppKit
-  NSAnimationEffect Deprecated

Enumeration

# NSAnimationEffect

The type for standard system animation effects, which include both display and sound.

macOS 10.3–14.0Deprecated

``` source
enum NSAnimationEffect
```

Deprecated

Use +\[NSCursor disappearingItemCursor\] instead

## Overview

These effects are used to indicate that an item was removed from a collection, such as a toolbar, without deleting the underlying data. See NSShowAnimationEffect.

## Topics

### Constants

case disappearingItemDefault

The default effect.

case poof

An effect showing a puff of smoke.

### Instance Methods

func show(centeredAt: NSPoint, size: NSSize, completionHandler: () -> Void)

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### View-Based Animations

class NSViewAnimation

An animation of an app’s views, limited to changes in frame location and size, and to fade-in and fade-out effects.

protocol NSAnimatablePropertyContainer

A set of methods that defines a way to add animation to an existing class with a minimum of API impact.

class NSAnimationContext

An animation context, which contains information about environment and state.

typealias Progress

The animation progress, as a floating-point number between `0.0` and `1.0`.

