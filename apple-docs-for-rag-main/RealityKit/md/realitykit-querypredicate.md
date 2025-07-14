

- RealityKit
-  QueryPredicate 

Structure

# QueryPredicate

An object that defines the criteria for an entity query.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct QueryPredicate
```

## Mentioned in 

Implementing systems for entities in a scene

## Overview

Query predicates specify the entities an EntityQuery returns from a scene. Predicates describe entities based on which components they contain, or on the entity’s relationship to other entities in the scene. For example, you can build a predicate to retrieve the model entities from a scene.

```
let modelPredicate = QueryPredicate.has(ModelComponent.self)
```

### Create compound predicates

You can combine predicates using Swift’s logical operators to create compound predicates. QueryPredicate supports Swift’s logical `AND` (`&&`), logical `OR` (`||`), and logical `NOT` (`!`) operators. The following code shows how to build a compound predicate that returns all entities that are either model entities or anchor entities:

```
let orPredicate: QueryPredicate =
    .has(ModelComponent.self) || .has(AnchorComponent.self)
```

Use parentheses to control the order of operations when combining predicates. For example, you can create a query that returns any entity that has both a model component and a physics body component, or any entity that has only an anchor component.

```
let multiPredicate: QueryPredicate =
    .has(ModelComponent.self) && .has(PhysicsBodyComponent.self) ||
    .has(AnchorComponent.self)
```

## Topics

### Creating predicates

static func has&lt;T>(T.Type) -> QueryPredicate&lt;Entity>

Creates a new predicate that describes entities that have a specific component.

### Comparing predicates

func ! &lt;Value>(QueryPredicate&lt;Value>) -> QueryPredicate&lt;Value>

Returns a predicate which evaluates to `true` if `operand` evaluates to `false`.

func &amp;&amp; &lt;Value>(QueryPredicate&lt;Value>, QueryPredicate&lt;Value>) -> QueryPredicate&lt;Value>

Returns a predicate which evaluates to `true` if `left` AND `right` evaluate to `true`.

func || &lt;Value>(QueryPredicate&lt;Value>, QueryPredicate&lt;Value>) -> QueryPredicate&lt;Value>

Returns a predicate which evaluates to `true` if `left` OR `right` evaluates to `true`.

## See Also

### Entity searches

struct PixelCastHit

