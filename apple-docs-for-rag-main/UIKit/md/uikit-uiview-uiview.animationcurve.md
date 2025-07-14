

- UIKit
- UIView
-  UIView.AnimationCurve 

Enumeration

# UIView.AnimationCurve

Specifies the supported animation curves.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum AnimationCurve
```

## Topics

### Constants

case easeInOut

An ease-in ease-out curve causes the animation to begin slowly, accelerate through the middle of its duration, and then slow again before completing. This is the default curve for most animations.

case easeIn

An ease-in curve causes the animation to begin slowly, and then speed up as it progresses.

case easeOut

An ease-out curve causes the animation to begin quickly, and then slow down as it completes.

case linear

A linear animation curve causes an animation to occur evenly over its duration.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct AnimationOptions

Options for animating views using block objects.

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

