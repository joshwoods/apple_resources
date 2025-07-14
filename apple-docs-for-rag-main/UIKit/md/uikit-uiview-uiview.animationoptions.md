

- UIKit
- UIView
-  UIView.AnimationOptions 

Structure

# UIView.AnimationOptions

Options for animating views using block objects.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
struct AnimationOptions
```

## Topics

### Constants

static var layoutSubviews: UIView.AnimationOptions

Lay out subviews at commit time so that they are animated along with their parent.

static var allowUserInteraction: UIView.AnimationOptions

Allow the user to interact with views while they are being animated.

static var beginFromCurrentState: UIView.AnimationOptions

Start the animation from the current setting associated with an already in-flight animation.

static var `repeat`: UIView.AnimationOptions

Repeat the animation indefinitely.

static var autoreverse: UIView.AnimationOptions

Run the animation backwards and forwards (must be combined with the repeat option).

static var overrideInheritedDuration: UIView.AnimationOptions

Force the animation to use the original duration value specified when the animation was submitted.

static var overrideInheritedCurve: UIView.AnimationOptions

Force the animation to use the original curve value specified when the animation was submitted.

static var allowAnimatedContent: UIView.AnimationOptions

Animate the views by changing the property values dynamically and redrawing the view.

static var showHideTransitionViews: UIView.AnimationOptions

Hide or show views during a view transition.

static var overrideInheritedOptions: UIView.AnimationOptions

The option to not inherit the animation type or any options.

static var curveEaseInOut: UIView.AnimationOptions

Specify an ease-in ease-out curve, which causes the animation to begin slowly, accelerate through the middle of its duration, and then slow again before completing.

static var curveEaseIn: UIView.AnimationOptions

An ease-in curve causes the animation to begin slowly, and then speed up as it progresses.

static var curveEaseOut: UIView.AnimationOptions

An ease-out curve causes the animation to begin quickly, and then slow as it completes.

static var curveLinear: UIView.AnimationOptions

A linear animation curve causes an animation to occur evenly over its duration.

static var transitionFlipFromLeft: UIView.AnimationOptions

A transition that flips a view around its vertical axis from left to right (the left side of the view moves toward the front and right side toward the back).

static var transitionFlipFromRight: UIView.AnimationOptions

A transition that flips a view around its vertical axis from right to left (the right side of the view moves toward the front and left side toward the back).

static var transitionCurlUp: UIView.AnimationOptions

A transition that curls a view up from the bottom.

static var transitionCurlDown: UIView.AnimationOptions

A transition that curls a view down from the top.

static var transitionCrossDissolve: UIView.AnimationOptions

A transition that dissolves from one view to the next.

static var transitionFlipFromTop: UIView.AnimationOptions

A transition that flips a view around its horizontal axis from top to bottom (the top side of the view moves toward the front and the bottom side toward the back).

static var transitionFlipFromBottom: UIView.AnimationOptions

A transition that flips a view around its horizontal axis from bottom to top (the bottom side of the view moves toward the front and the top side toward the back).

static var preferredFramesPerSecond30: UIView.AnimationOptions

A frame rate of 30 frames per second.

static var preferredFramesPerSecond60: UIView.AnimationOptions

A frame rate of 60 frames per second.

### Initializers

init(rawValue: UInt)

Creates an animation options structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

enum AnimationCurve

Specifies the supported animation curves.

enum AnimationTransition

Animation transition options for use in an animation block object.

enum SystemAnimation

Option to remove the views from the hierarchy when animation is complete.

struct KeyframeAnimationOptions

Options for configuring keyframe-based animations.

enum Axis

Keys that specify a horizontal or vertical layout constraint between objects.

enum TintAdjustmentMode

The tint adjustment mode for the view.

class let layoutFittingCompressedSize: CGSize

The option to use the smallest possible size.

class let layoutFittingExpandedSize: CGSize

The option to use the largest possible size.

class let noIntrinsicMetric: CGFloat

The absence of an intrinsic metric for a given numeric view property.

struct AutoresizingMask

Options for automatic view resizing.

enum UISemanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

