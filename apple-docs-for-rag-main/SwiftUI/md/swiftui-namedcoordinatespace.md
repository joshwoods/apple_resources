

- SwiftUI
-  NamedCoordinateSpace 

Structure

# NamedCoordinateSpace

A named coordinate space.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct NamedCoordinateSpace
```

## Overview

Use the `coordinateSpace(_:)` modifier to assign a name to the local coordinate space of a parent view. Child views can then refer to that coordinate space using `.named(_:)`.

## Relationships

### Conforms To

- CoordinateSpaceProtocol
- Equatable

## See Also

### Supporting types

struct GlobalCoordinateSpace

The global coordinate space at the root of the view hierarchy.

struct LocalCoordinateSpace

The local coordinate space of the current view.

