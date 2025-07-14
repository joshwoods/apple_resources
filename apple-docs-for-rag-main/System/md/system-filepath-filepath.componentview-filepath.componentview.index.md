

- System
- FilePath
- FilePath.ComponentView
-  FilePath.ComponentView.Index 

Structure

# FilePath.ComponentView.Index

A type that represents a position in the collection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Index
```

## Overview

Valid indices consist of the position of every element and a “past the end” position that’s not valid for use as a subscript argument.

## Topics

### Operators

static func == (FilePath.ComponentView.Index, FilePath.ComponentView.Index) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (FilePath.ComponentView.Index, FilePath.ComponentView.Index) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Comparable
- Equatable
- Hashable
- Sendable

