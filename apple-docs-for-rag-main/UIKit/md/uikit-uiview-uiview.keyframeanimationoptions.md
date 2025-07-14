

- UIKit
- UIView
-  UIView.KeyframeAnimationOptions 

Structure

# UIView.KeyframeAnimationOptions

Options for configuring keyframe-based animations.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
struct KeyframeAnimationOptions
```

## Overview

Use these options with the animateKeyframes(withDuration:delay:options:animations:completion:) method.

## Topics

### Constants

static var layoutSubviews: UIView.KeyframeAnimationOptions

The option to lay out subviews at commit time so that they’re animated along with their parent.

static var allowUserInteraction: UIView.KeyframeAnimationOptions

The option that allows a person to interact with views while they’re being animated.

static var beginFromCurrentState: UIView.KeyframeAnimationOptions

The option to start an animation from the current setting associated with an already in-flight animation.

static var `repeat`: UIView.KeyframeAnimationOptions

The option to repeat an animation indefinitely.

static var autoreverse: UIView.KeyframeAnimationOptions

The option to run an animation backwards and forwards.

static var overrideInheritedDuration: UIView.KeyframeAnimationOptions

The option to force an animation to use the original duration value specified when the animation was submitted.

static var overrideInheritedOptions: UIView.KeyframeAnimationOptions

The option to not inherit the animation type or any options.

static var calculationModeLinear: UIView.KeyframeAnimationOptions

The option to use a simple linear calculation when interpolating between keyframe values.

static var calculationModeDiscrete: UIView.KeyframeAnimationOptions

The option to not interpolate between keyframe values, but rather to jump directly to each new keyframe value.

static var calculationModePaced: UIView.KeyframeAnimationOptions

The option to compute intermediate keyframe values using a simple pacing algorithm.

static var calculationModeCubic: UIView.KeyframeAnimationOptions

The option to compute intermediate frames using a default Catmull-Rom spline that passes through the keyframe values.

static var calculationModeCubicPaced: UIView.KeyframeAnimationOptions

The option to compute intermediate frames using the cubic scheme while ignoring the timing properties of the animation.

### Initializers

init(rawValue: UInt)

Creates keyframe animation options with the specified raw value.

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

struct AnimationOptions

Options for animating views using block objects.

enum AnimationTransition

Animation transition options for use in an animation block object.

enum SystemAnimation

Option to remove the views from the hierarchy when animation is complete.

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

