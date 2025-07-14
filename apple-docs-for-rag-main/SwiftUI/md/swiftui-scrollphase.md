

- SwiftUI
-  ScrollPhase 

Enumeration

# ScrollPhase

A type that describes the state of a scroll gesture of a scrollable view like a scroll view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
@frozen
enum ScrollPhase
```

## Overview

A scroll gesture can be in one of four phases: - idle: No active scroll is occurring. - panning: An active scroll being driven by the user is occurring. - decelerating: The user has stopped driving a scroll and the scroll view is decelerating to its final target. - animating: The system is animating to a final target as a result of a programmatic animated scroll from using a ScrollViewReader or scrollPosition(id:anchor:) modifier.

SwiftUI provides you a value of this type when using the onScrollPhaseChange(_:) modifier.

## Topics

### Getting scroll gesture states

case animating

The animating phase where the scroll view is animating towards a final target.

case decelerating

The decelerating phase where the user use has stopped interacting with the scroll view and the scroll view is decelerating towards its final target.

case idle

The idle phase where no kind of scrolling is occurring.

case interacting

The interacting phase where the user is interacting with the scroll view.

case tracking

The tracking phase where the scroll view is tracking a potential scroll by the user but the user hasn’t started a scroll.

### Checking for active scrolling

var isScrolling: Bool

Whether the scroll view is actively scrolling.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
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

struct ScrollGeometry

A type that defines the geometry of a scroll view.

struct ScrollPhaseChangeContext

A type that provides you with more content when the phase of a scroll view changes.

