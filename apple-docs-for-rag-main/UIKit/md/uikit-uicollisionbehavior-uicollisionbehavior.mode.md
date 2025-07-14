

- UIKit
- UICollisionBehavior
-  UICollisionBehavior.Mode 

Structure

# UICollisionBehavior.Mode

The types of edges that participate in collisions for a collision behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
struct Mode
```

## Topics

### Constants

static var items: UICollisionBehavior.Mode

Specifies that the dynamic items, associated with the collision behavior, collide only with each other and not with specified collision boundaries.

static var boundaries: UICollisionBehavior.Mode

Specifies that the dynamic items, associated with the collision behavior, collide only with specified collision boundaries and don’t collide with each other.

static var everything: UICollisionBehavior.Mode

Specifies that the dynamic items, associated with the collision behavior, collide with each other *and* with specified collision boundaries.

### Initializers

init(rawValue: UInt)

Creates a collision behavior mode structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

