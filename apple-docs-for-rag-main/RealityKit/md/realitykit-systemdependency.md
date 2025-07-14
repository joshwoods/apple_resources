

- RealityKit
-  SystemDependency 

Enumeration

# SystemDependency

Defines update order relative to other systems. An object that specifies the update order between multiple systems.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum SystemDependency
```

## Overview

Add instances of `SystemDependency` to your system’s dependencies array to indicate whether RealityKit updates another specified system before or after this system.

## Topics

### Update order

case before(any System.Type)

An update order that requests RealityKit update this system before it updates another specified system.

case after(any System.Type)

An update order that requests RealityKit update this system after it updates another specified system.

### Comparisons

static func == (SystemDependency, SystemDependency) -> Bool

Returns a Boolean value that indicates whether two dependencies are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Specifying dependencies

static var dependencies: [SystemDependency]

An array of dependencies for this system.

**Required** Default implementation provided.

