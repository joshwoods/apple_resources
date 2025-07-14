

- UIKit
-  UISemanticContentAttribute 

Enumeration

# UISemanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
enum UISemanticContentAttribute
```

## Topics

### Constants

case unspecified

The default value for views.

case playback

A view representing the playback controls, such as Play, Rewind, or Fast Forward buttons or playhead scrubbers.

case spatial

A view representing a directional control, such as a segment control for text alignment, or a D-pad control for a game.

case forceLeftToRight

A view that’s always displayed using a left-to-right layout.

case forceRightToLeft

A view that’s always displayed using a right-to-left layout.

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

