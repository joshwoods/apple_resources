

- Create ML
- MLDataValue
- MLDataValue.DictionaryType
-  MLDataValue.DictionaryType.Index 

Structure

# MLDataValue.DictionaryType.Index

A type that represents a position in the collection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct Index
```

## Overview

Valid indices consist of the position of every element and a “past the end” position that’s not valid for use as a subscript argument.

## Topics

### Comparing dictionary types

static func == (MLDataValue.DictionaryType.Index, MLDataValue.DictionaryType.Index) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (MLDataValue.DictionaryType.Index, MLDataValue.DictionaryType.Index) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Comparable
- Equatable

