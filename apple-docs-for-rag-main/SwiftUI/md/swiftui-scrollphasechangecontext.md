

- SwiftUI
-  ScrollPhaseChangeContext 

Structure

# ScrollPhaseChangeContext

A type that provides you with more content when the phase of a scroll view changes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct ScrollPhaseChangeContext
```

## Overview

You don’t create this type directly. Instead, SwiftUI provides an instance of this type in the onScrollPhaseChange(_:) modifier.

## Topics

### Instance Properties

var geometry: ScrollGeometry

The geometry of the scroll view at the time of the scroll phase change.

var velocity: CGVector?

The velocity of the scroll view at the time of the scroll phase change.

## See Also

### Responding to scroll view changes

func onScrollGeometryChange&lt;T>(for: T.Type, of: (ScrollGeometry) -> T, action: (T, T) -> Void) -> some View

Adds an action to be performed when a value, created from a scroll geometry, changes.

func onScrollTargetVisibilityChange&lt;ID>(idType: ID.Type, threshold: Double, ([ID]) -> Void) -> some View

Adds an action to be called with information about what views would be considered visible.

func onScrollVisibilityChange(threshold: Double, (Bool) -> Void) -> some View

Adds an action to be called when the view crosses the threshold to be considered on/off screen.

func onScrollPhaseChange(_:)

Adds an action to perform when the scroll phase of the first scroll view in the hierarchy changes.

struct ScrollGeometry

A type that defines the geometry of a scroll view.

enum ScrollPhase

A type that describes the state of a scroll gesture of a scrollable view like a scroll view.

