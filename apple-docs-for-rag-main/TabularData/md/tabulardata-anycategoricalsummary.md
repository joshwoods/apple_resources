

- TabularData
-  AnyCategoricalSummary 

Structure

# AnyCategoricalSummary

A type-erased categorical summary.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AnyCategoricalSummary
```

## Overview

Categorical summary includes 5 statistics:

- someCount: The number of non-missing elements.

- noneCount: The number of missing elements.

- totalCount: The sum of missing and non-missing elements.

- uniqueCount: The number of unique elements.

- mode: The most common elements.

## Topics

### Getting Statistical Information

var noneCount: Int

The number of missing elements in the column.

var someCount: Int

The number of non-missing elements in the column.

var totalCount: Int

The total number of elements in the column.

var uniqueCount: Int

The number of unique elements.

### Getting Mode Information

var mode: [Any]

The most common values in a column.

var modeType: any Any.Type

The underlying type of mode.

### Operators

static func == (AnyCategoricalSummary, AnyCategoricalSummary) -> Bool

Returns a Boolean value that indicates whether the categorical summaries are equal.

### Initializers

init(CategoricalSummary&lt;AnyHashable>)

Creates a type-erased categorical summary from a typed categorical summary.

init&lt;T>(CategoricalSummary&lt;T>)

Creates a type-erased categorical summary from a typed categorical summary.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Statistical Summaries

struct NumericSummary

A summary of a numerical column.

struct CategoricalSummary

A categorical summary of a collection’s elements.

