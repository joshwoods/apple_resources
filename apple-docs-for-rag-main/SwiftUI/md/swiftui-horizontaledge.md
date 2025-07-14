

- SwiftUI
-  HorizontalEdge 

Enumeration

# HorizontalEdge

An edge on the horizontal axis.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum HorizontalEdge
```

## Overview

Use a horizontal edge for tasks like setting a swipe action with the swipeActions(edge:allowsFullSwipe:content:) view modifier. The positions of the leading and trailing edges depend on the locale chosen by the user.

## Topics

### Getting the edges

case leading

The leading edge.

case trailing

The trailing edge.

### Accessing sets of edges

struct Set

An efficient set of horizontal edges.

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing edges and regions

enum Edge

An enumeration to indicate one edge of a rectangle.

enum Edge3D

An edge or face of a 3D volume.

enum VerticalEdge

An edge on the vertical axis.

struct EdgeInsets

The inset distances for the sides of a rectangle.

struct EdgeInsets3D

The inset distances for the faces of a 3D volume.

