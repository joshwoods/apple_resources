

- SwiftUI
-  UnitCurve 

Structure

# UnitCurve

A function defined by a two-dimensional curve that maps an input progress in the range \[0,1\] to an output progress that is also in the range \[0,1\]. By changing the shape of the curve, the effective speed of an animation or other interpolation can be changed.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct UnitCurve
```

## Overview

The horizontal (x) axis defines the input progress: a single input progress value in the range \[0,1\] must be provided when evaluating a curve.

The vertical (y) axis maps to the output progress: when a curve is evaluated, the y component of the point that intersects the input progress is returned.

## Topics

### Getting a linear curve

static let linear: UnitCurve

A linear curve.

### Getting easing curves

static let easeIn: UnitCurve

A bezier curve that starts out slowly, then speeds up as it finishes.

static let easeOut: UnitCurve

A bezier curve that starts out quickly, then slows down as it approaches the end.

static let easeInOut: UnitCurve

A bezier curve that starts out slowly, speeds up over the middle, then slows down again as it approaches the end.

static let circularEaseIn: UnitCurve

A curve that starts out slowly, then speeds up as it finishes.

static let circularEaseOut: UnitCurve

A circular curve that starts out quickly, then slows down as it approaches the end.

static let circularEaseInOut: UnitCurve

A circular curve that starts out slowly, speeds up over the middle, then slows down again as it approaches the end.

### Creating a general Bezier curve

static func bezier(startControlPoint: UnitPoint, endControlPoint: UnitPoint) -> UnitCurve

Creates a new curve using bezier control points.

### Inverting a curve

var inverse: UnitCurve

Returns a copy of the curve with its x and y components swapped.

### Getting curve characteristics

func value(at: Double) -> Double

Returns the output value (y component) of the curve at the given time.

func velocity(at: Double) -> Double

Returns the rate of change (first derivative) of the output value of the curve at the given time.

### Deprecated symbols

static let easeInEaseOut: UnitCurve

A bezier curve that starts out slowly, speeds up over the middle, then slows down again as it approaches the end.

Deprecated

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating custom animations

protocol CustomAnimation

A type that defines how an animatable value changes over time.

struct AnimationContext

Contextual values that a custom animation can use to manage state and access a view’s environment.

struct AnimationState

A container that stores the state for a custom animation.

protocol AnimationStateKey

A key for accessing animation state values.

struct Spring

A representation of a spring’s motion.

