

- SwiftUI
-  SensoryFeedback 

Structure

# SensoryFeedback

Represents a type of haptic and/or audio feedback that can be played.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
struct SensoryFeedback
```

## Overview

This feedback can be passed to `View.sensoryFeedback` to play it.

## Topics

### Indicating start and stop

static let start: SensoryFeedback

Indicates that an activity started.

static let stop: SensoryFeedback

Indicates that an activity stopped.

### Indicating changes and selections

static let alignment: SensoryFeedback

Indicates the alignment of a dragged item.

static let decrease: SensoryFeedback

Indicates that an important value decreased below a significant threshold.

static let increase: SensoryFeedback

Indicates that an important value increased above a significant threshold.

static let levelChange: SensoryFeedback

Indicates movement between discrete levels of pressure.

static let selection: SensoryFeedback

Indicates that a UI element’s values are changing.

static let pathComplete: SensoryFeedback

Indicates a drawn path has completed and/or recognized.

### Indicating the outcome of an operation

static let success: SensoryFeedback

Indicates that a task or action has completed.

static let warning: SensoryFeedback

Indicates that a task or action has produced a warning of some kind.

static let error: SensoryFeedback

Indicates that an error has occurred.

### Producing a physical impact

static let impact: SensoryFeedback

Provides a physical metaphor you can use to complement a visual experience.

static func impact(weight: SensoryFeedback.Weight, intensity: Double) -> SensoryFeedback

Provides a physical metaphor you can use to complement a visual experience.

static func impact(flexibility: SensoryFeedback.Flexibility, intensity: Double) -> SensoryFeedback

Provides a physical metaphor you can use to complement a visual experience.

struct Flexibility

The flexibility to be represented by a type of feedback.

struct Weight

The weight to be represented by a type of feedback.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Providing haptic feedback

func sensoryFeedback&lt;T>(SensoryFeedback, trigger: T) -> some View

Plays the specified `feedback` when the provided `trigger` value changes.

func sensoryFeedback&lt;T>(trigger: T, (T, T) -> SensoryFeedback?) -> some View

Plays feedback when returned from the `feedback` closure after the provided `trigger` value changes.

func sensoryFeedback&lt;T>(SensoryFeedback, trigger: T, condition: (T, T) -> Bool) -> some View

Plays the specified `feedback` when the provided `trigger` value changes and the `condition` closure returns `true`.

