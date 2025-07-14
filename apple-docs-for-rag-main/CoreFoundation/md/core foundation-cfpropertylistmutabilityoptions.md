

- Core Foundation
-  CFPropertyListMutabilityOptions 

Structure

# CFPropertyListMutabilityOptions

Type for flags that determine the degree of mutability of newly created property lists.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFPropertyListMutabilityOptions
```

## Overview

See Property List Mutability Options for possible values.

## Topics

### Initializers

init(rawValue: CFOptionFlags)

### Type Properties

static var mutableContainers: CFPropertyListMutabilityOptions

Specifies that the property list should have mutable containers but immutable leaves.

static var mutableContainersAndLeaves: CFPropertyListMutabilityOptions

Specifies that the property list should have mutable containers and mutable leaves.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

