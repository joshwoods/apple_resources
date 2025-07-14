

- SwiftUI
-  Namespace 

Structure

# Namespace

A dynamic property type that allows access to a namespace defined by the persistent identity of the object containing the property (e.g. a view).

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen @propertyWrapper
struct Namespace
```

## Topics

### Creating a namespace

init()

### Getting the namespace

var wrappedValue: Namespace.ID

struct ID

A namespace defined by the persistent identity of an `@Namespace` dynamic property.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- DynamicProperty
- Sendable

## See Also

### Synchronizing geometries

func matchedGeometryEffect&lt;ID>(id: ID, in: Namespace.ID, properties: MatchedGeometryProperties, anchor: UnitPoint, isSource: Bool) -> some View

Defines a group of views with synchronized geometry using an identifier and namespace that you provide.

struct MatchedGeometryProperties

A set of view properties that may be synchronized between views using the `View.matchedGeometryEffect()` function.

protocol GeometryEffect

An effect that changes the visual appearance of a view, largely without changing its ancestors or descendants.

func geometryGroup() -> some View

Isolates the geometry (e.g. position and size) of the view from its parent view.

