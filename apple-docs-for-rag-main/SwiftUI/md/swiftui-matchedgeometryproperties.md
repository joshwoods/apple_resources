

- SwiftUI
-  MatchedGeometryProperties 

Structure

# MatchedGeometryProperties

A set of view properties that may be synchronized between views using the `View.matchedGeometryEffect()` function.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen
struct MatchedGeometryProperties
```

## Topics

### Matching properties

static let frame: MatchedGeometryProperties

Both the `position` and `size` properties.

static let position: MatchedGeometryProperties

The view’s position, in window coordinates.

static let size: MatchedGeometryProperties

The view’s size, in local coordinates.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Synchronizing geometries

func matchedGeometryEffect&lt;ID>(id: ID, in: Namespace.ID, properties: MatchedGeometryProperties, anchor: UnitPoint, isSource: Bool) -> some View

Defines a group of views with synchronized geometry using an identifier and namespace that you provide.

protocol GeometryEffect

An effect that changes the visual appearance of a view, largely without changing its ancestors or descendants.

struct Namespace

A dynamic property type that allows access to a namespace defined by the persistent identity of the object containing the property (e.g. a view).

func geometryGroup() -> some View

Isolates the geometry (e.g. position and size) of the view from its parent view.

