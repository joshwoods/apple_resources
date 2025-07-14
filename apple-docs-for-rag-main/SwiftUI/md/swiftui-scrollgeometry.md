

- SwiftUI
-  ScrollGeometry 

Structure

# ScrollGeometry

A type that defines the geometry of a scroll view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct ScrollGeometry
```

## Overview

SwiftUI provides you values of this type when using modifiers like `View/onScrollGeometryChange(_:action:)` or onScrollPhaseChange(_:).

## Topics

### Initializers

init(contentOffset: CGPoint, contentSize: CGSize, contentInsets: EdgeInsets, containerSize: CGSize)

Creates a scroll geometry.

### Instance Properties

var bounds: CGRect

The bounds rect of the scroll view.

var containerSize: CGSize

The size of the container of the scroll view.

var contentInsets: EdgeInsets

The content insets of the scroll view.

var contentOffset: CGPoint

The content offset of the scroll view.

var contentSize: CGSize

The size of the content of the scroll view.

var visibleRect: CGRect

The visible rect of the scroll view.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Sendable

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

enum ScrollPhase

A type that describes the state of a scroll gesture of a scrollable view like a scroll view.

struct ScrollPhaseChangeContext

A type that provides you with more content when the phase of a scroll view changes.

