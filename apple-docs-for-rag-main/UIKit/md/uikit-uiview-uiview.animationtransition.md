

- UIKit
- UIView
-  UIView.AnimationTransition 

Enumeration

# UIView.AnimationTransition

Animation transition options for use in an animation block object.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum AnimationTransition
```

## Topics

### Constants

case none

The option for indicating that no transition is specified.

case flipFromLeft

A transition that flips a view around a vertical axis from left to right. The left side of the view moves towards the front and right side towards the back.

case flipFromRight

A transition that flips a view around a vertical axis from right to left. The right side of the view moves towards the front and left side towards the back.

case curlUp

A transition that curls a view up from the bottom.

case curlDown

A transition that curls a view down from the top.

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

