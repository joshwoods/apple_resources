

- PackageDescription
- Package
- Package.Dependency
- Package.Dependency.Trait
-  Package.Dependency.Trait.Condition 

Structure

# Package.Dependency.Trait.Condition

A condition that limits the application of a dependencies trait.

SwiftPM 6.1+

``` source
struct Condition
```

## Topics

### Operators

static func == (Package.Dependency.Trait.Condition, Package.Dependency.Trait.Condition) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Methods

static func when(traits: Set&lt;String>) -> Package.Dependency.Trait.Condition?

Creates a package dependency trait condition.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

