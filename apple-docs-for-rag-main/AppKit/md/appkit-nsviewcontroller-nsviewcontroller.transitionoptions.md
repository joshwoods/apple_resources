

- AppKit
- NSViewController
-  NSViewController.TransitionOptions 

Structure

# NSViewController.TransitionOptions

Animation options for view transitions in a view controller.

macOS 10.10+

``` source
struct TransitionOptions
```

## Overview

The up and down slide animation options are disjoint and you cannot combine them.

Likewise, the left and right slide animation options are disjoint and you cannot combine them.

User interaction with transitioning views is prevented for all animation options except the allowUserInteraction option.

## Topics

### Constants

static var crossfade: NSViewController.TransitionOptions

A transition animation that fades the new view in and simultaneously fades the old view out. You can combine this animation option with any of the “slide” options in this enumeration.

static var slideUp: NSViewController.TransitionOptions

A transition animation that slides the old view up while the new view comes into view from the bottom. In other words, both views slide up.

static var slideDown: NSViewController.TransitionOptions

A transition animation that slides the old view down while the new view slides into view from the top. In other words, both views slide down.

static var slideLeft: NSViewController.TransitionOptions

A transition animation that slides the old view to the left while the new view slides into view from the right. In other words, both views slide to the left.

static var slideRight: NSViewController.TransitionOptions

A transition animation that slides the old view to the right while the new view slides into view from the left. In other words, both views slide to the right.

static var slideForward: NSViewController.TransitionOptions

A transition animation that reflects the user interface layout direction (userInterfaceLayoutDirection) in a “forward” manner, as follows:

static var slideBackward: NSViewController.TransitionOptions

A transition animation that reflects the user interface layout direction (userInterfaceLayoutDirection) in a “backward” manner, as follows

static var allowUserInteraction: NSViewController.TransitionOptions

A transition animation that allows user interaction during the transition.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

