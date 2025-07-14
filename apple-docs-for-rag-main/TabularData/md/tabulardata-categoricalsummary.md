

- TabularData
-  CategoricalSummary 

Structure

# CategoricalSummary

A categorical summary of a collection’s elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct CategoricalSummary where Element : Hashable
```

## Overview

Each categorical summary has 5 statistics about a collection:

- `someCount`: The number of non-missing elements.

- `noneCount` The number of missing elements.

- `uniqueCount`: The number of unique elements.

- `totalCount`: The total number of elements.

- `mode`: An array of the most common values.

## Topics

### Creating a Summary

init()

Creates a categorical summary with default values.

init(someCount: Int, noneCount: Int, uniqueCount: Int, mode: [Element])

Creates a categorical summary.

### Comparing Summaries

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Inspecting a Summary

var debugDescription: String

A text representation of the summary’s statistics suitable for debugging.

var mode: [Element]

The most common values in a column, ignoring missing elements.

var uniqueCount: Int

The number of elements with distinct values in a column that excludes missing elements.

var someCount: Int

The number of non-missing elements in the column.

var noneCount: Int

The number of missing elements in the column.

var totalCount: Int

The total number of elements in the column.

### Operators

static func == (CategoricalSummary&lt;Element>, CategoricalSummary&lt;Element>) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Statistical Summaries

struct NumericSummary

A summary of a numerical column.

struct AnyCategoricalSummary

A type-erased categorical summary.

