

- PackageDescription
-  TargetDependencyCondition 

Structure

# TargetDependencyCondition

A condition that limits the application of a target’s dependency.

``` source
struct TargetDependencyCondition
```

## Topics

### Creating a Dependency Condition

static func when(platforms: [Platform]) -> TargetDependencyCondition?

Creates a target dependency condition.

static func when(platforms: [Platform]?) -> TargetDependencyCondition

Creates a target dependency condition.

Deprecated

### Type Methods

static func when(platforms: [Platform], traits: Set&lt;String>) -> TargetDependencyCondition?

Creates a target dependency condition.

static func when(traits: Set&lt;String>) -> TargetDependencyCondition?

Creates a target dependency condition.

## Relationships

### Conforms To

- Sendable

## See Also

### Declaring a Dependency Target

var dependencies: [Target.Dependency]

The target’s dependencies on other entities inside or outside the package.

enum Dependency

The different types of a target’s dependency on another entity.

