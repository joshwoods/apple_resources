

- RealityKit
- Entity
- Entity.ComponentSet
-  Entity.ComponentSet.Index 

Structure

# Entity.ComponentSet.Index

A type that represents a position in the collection.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Index
```

## Overview

Valid indices consist of the position of every element and a “past the end” position that’s not valid for use as a subscript argument.

## Topics

### Operators

static func == (Entity.ComponentSet.Index, Entity.ComponentSet.Index) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (Entity.ComponentSet.Index, Entity.ComponentSet.Index) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Comparable
- Equatable
- Sendable

