

- AppKit
-  NSAnimationContext 

Class

# NSAnimationContext

An animation context, which contains information about environment and state.

macOS 10.5+

``` source
class NSAnimationContext
```

## Overview

NSAnimationContext is analogous to CATransaction and is similar in overall concept to NSGraphicsContext. Each thread maintains its own stack of nestable NSAnimationContext instances, with each new instance initialized as a copy of the instance below (so, inheriting its current properties).

Multiple NSAnimationContext instances can be nested, allowing a given block of code to initiate animations using its own specified duration without affecting animations initiated by surrounding code.

```
[NSAnimationContext beginGrouping];
// Animate enclosed operations with a duration of 1 second
[[NSAnimationContext currentContext] setDuration:1.0];
[[aView animator] setFrame:newFrame];
...
    [NSAnimationContext beginGrouping];
    // Animate alpha fades with half-second duration
    [[NSAnimationContext currentContext] setDuration:0.5];
    [[aView animator] setAlphaValue:0.75];
    [[bView animator] setAlphaValue:0.75];
    [NSAnimationContext endGrouping];
...
// Will animate with a duration of 1 second
[[bView animator] setFrame:secondFrame];
[NSAnimationContext endGrouping];
```

## Topics

### Grouping Transactions

class func beginGrouping()

Creates a new animation grouping.

class func endGrouping()

Ends the current animation grouping.

### Getting the Current Animation Context

class var current: NSAnimationContext

Returns the current animation context.

### Animation Completion Handlers

var completionHandler: (() -> Void)?

A completion Block that is called when the animations in the grouping are completed.

class func runAnimationGroup((NSAnimationContext) -> Void, completionHandler: (() -> Void)?)

Allows you to specify a completion block body after the set of animation actions whose completion will trigger the completion block.

### Modifying the Animation Duration

var duration: TimeInterval

The duration used by animations created as a result of setting new values for an animatable property.

var timingFunction: CAMediaTimingFunction?

The timing function used for all animations within this animation proxy group.

### Implicit Animation

var allowsImplicitAnimation: Bool

Determine if animations are enabled or not for animations that occur as a result of another property change.

### Type Methods

class func runAnimationGroup((NSAnimationContext) -> Void)

static func animate(Animation, changes: () -> Void, completion: (() -> Void)?)

Animate changes to one or more views using the specified SwiftUI animation.

static func animate(with: Animation, changes: () -> Void, completion: (() -> Void)?)

Animates changes to one or more views using the specified SwiftUI animation.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### View-Based Animations

class NSViewAnimation

An animation of an app’s views, limited to changes in frame location and size, and to fade-in and fade-out effects.

protocol NSAnimatablePropertyContainer

A set of methods that defines a way to add animation to an existing class with a minimum of API impact.

typealias Progress

The animation progress, as a floating-point number between `0.0` and `1.0`.

enum NSAnimationEffect

The type for standard system animation effects, which include both display and sound.

Deprecated

