

- UIKit
- UIView
-  UIView.TintAdjustmentMode 

Enumeration

# UIView.TintAdjustmentMode

The tint adjustment mode for the view.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum TintAdjustmentMode
```

## Topics

### Constants

case automatic

The tint adjustment mode of the view is the same as its superview’s tint adjustment mode (or `UIViewTintAdjustmentModeNormal` if the view has no superview).

case normal

The view’s tint color property returns the completely unmodified tint color of the view.

case dimmed

The view’s tint color property returns a desaturated, dimmed version of the view’s original tint color.

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

enum AnimationCurve

Specifies the supported animation curves.

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

