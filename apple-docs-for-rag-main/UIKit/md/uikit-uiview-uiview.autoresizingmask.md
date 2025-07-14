

- UIKit
- UIView
-  UIView.AutoresizingMask 

Structure

# UIView.AutoresizingMask

Options for automatic view resizing.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct AutoresizingMask
```

## Topics

### Constants

static var flexibleLeftMargin: UIView.AutoresizingMask

Resizing performed by expanding or shrinking a view in the direction of the left margin.

static var flexibleWidth: UIView.AutoresizingMask

Resizing performed by expanding or shrinking a view’s width.

static var flexibleRightMargin: UIView.AutoresizingMask

Resizing performed by expanding or shrinking a view in the direction of the right margin.

static var flexibleTopMargin: UIView.AutoresizingMask

Resizing performed by expanding or shrinking a view in the direction of the top margin.

static var flexibleHeight: UIView.AutoresizingMask

Resizing performed by expanding or shrinking a view’s height.

static var flexibleBottomMargin: UIView.AutoresizingMask

Resizing performed by expanding or shrinking a view in the direction of the bottom margin.

### Initializers

init(rawValue: UInt)

Creates an autoresizing mask structure with the specified raw value.

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

enum UISemanticContentAttribute

A semantic description of the view’s contents, used to determine whether the view should be flipped when switching between left-to-right and right-to-left layouts.

