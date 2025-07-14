

- Foundation
-  SortComparator 

Protocol

# SortComparator

A comparison algorithm for a specified type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
protocol SortComparator : Hashable, Sendable
```

## Overview

Objects that conform to SortComparator provide a comparison algorithm and storage for the sort order to use when comparing.

## Topics

### Inspecting a Comparator

var order: SortOrder

The sort order that the comparator uses to compare.

**Required**

static var localized: String.Comparator

A comparator that compares a string using a localized comparison in the current locale.

static var localizedStandard: String.Comparator

A comparator that compares a string using a localized, numeric comparison in the current locale.

### Using a Comparator

func compare(Self.Compared, Self.Compared) -> ComparisonResult

Provides the relative ordering of two elements based on the sort order of the comparator.

**Required**

associatedtype Compared

A type that the sort comparator can compare.

**Required**

## Relationships

### Inherits From

- Equatable
- Hashable
- Sendable

### Conforming Types

- ComparableComparator
- KeyPathComparator
- SortDescriptor

## See Also

### Sorting

class NSSortDescriptor

An immutable description of how to order a collection of objects according to a property common to all the objects.

enum ComparisonResult

Constants that indicate sort order.

struct SortDescriptor

A serializable description of how to sort numerics and strings.

struct ComparableComparator

A comparator that compares types according to their conformance to the comparable protocol.

struct KeyPathComparator

A comparator that uses another sort comparator to provide the comparison of values at a key path.

enum SortOrder

The orderings that you can perform sorts with.

