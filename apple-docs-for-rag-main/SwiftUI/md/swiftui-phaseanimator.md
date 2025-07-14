

- SwiftUI
-  PhaseAnimator 

Structure

# PhaseAnimator

A container that animates its content by automatically cycling through a collection of phases that you provide, each defining a discrete step within an animation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct PhaseAnimator where Phase : Equatable, Content : View
```

## Overview

Use one of the phase animator view modifiers like phaseAnimator(_:content:animation:) to create a phased animation in your app.

## Topics

### Creating a phase animator

init(some Sequence&lt;Phase>, content: (Phase) -> Content, animation: (Phase) -> Animation?)

Cycles through a sequence of phases continuously, animating updates to a view on each phase change.

init(some Sequence&lt;Phase>, trigger: some Equatable, content: (Phase) -> Content, animation: (Phase) -> Animation?)

Cycles through a sequence of phases in response to changes in a specified value, animating updates to a view on each phase change.

## Relationships

### Conforms To

- View

## See Also

### Creating phase-based animation

Controlling the timing and movements of your animations

Build sophisticated animations that you control using phase and keyframe animators.

func phaseAnimator&lt;Phase>(some Sequence, content: (PlaceholderContentView&lt;Self>, Phase) -> some View, animation: (Phase) -> Animation?) -> some View

Animates effects that you apply to a view over a sequence of phases that change continuously.

func phaseAnimator&lt;Phase>(some Sequence, trigger: some Equatable, content: (PlaceholderContentView&lt;Self>, Phase) -> some View, animation: (Phase) -> Animation?) -> some View

Animates effects that you apply to a view over a sequence of phases that change based on a trigger.

