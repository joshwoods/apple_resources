

- Foundation
- PropertyListSerialization
-  PropertyListSerialization.MutabilityOptions 

Structure

# PropertyListSerialization.MutabilityOptions

These constants specify mutability options in property lists.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct MutabilityOptions
```

## Topics

### Constants

static var mutableContainers: PropertyListSerialization.MutabilityOptions

Causes the returned property list to have mutable containers but immutable leaves.

static var mutableContainersAndLeaves: PropertyListSerialization.MutabilityOptions

Causes the returned property list to have mutable containers and leaves.

static var mutableContainers: PropertyListSerialization.MutabilityOptions

Causes the returned property list to have mutable containers but immutable leaves.

static var mutableContainersAndLeaves: PropertyListSerialization.MutabilityOptions

Causes the returned property list to have mutable containers and leaves.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

enum PropertyListFormat

These constants are used to specify a property list serialization format.

typealias ReadOptions

The only read options supported are described in PropertyListSerialization.MutabilityOptions.

