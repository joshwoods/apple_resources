

- Foundation
- NSComparisonPredicate
-  NSComparisonPredicate.Options 

Structure

# NSComparisonPredicate.Options

Constants that describe the possible types of string comparison for comparison predicates.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Options
```

## Overview

The system supports these options for `LIKE`, as well as all of the equality/comparison operators.

## Topics

### Constants

static var caseInsensitive: NSComparisonPredicate.Options

A case-insensitive predicate.

static var diacriticInsensitive: NSComparisonPredicate.Options

A diacritic-insensitive predicate.

static var normalized: NSComparisonPredicate.Options

A predicate that indicates you’ve preprocessed the strings to compare.

static var caseInsensitive: NSComparisonPredicate.Options

A case-insensitive predicate.

static var diacriticInsensitive: NSComparisonPredicate.Options

A diacritic-insensitive predicate.

static var normalized: NSComparisonPredicate.Options

A predicate that indicates you’ve preprocessed the strings to compare.

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

### Getting Information About a Comparison Predicate

var comparisonPredicateModifier: NSComparisonPredicate.Modifier

The comparison predicate modifier for the receiver.

enum Modifier

Constants that describe the possible types of modifier for a comparison predicate.

var customSelector: Selector?

The selector for the receiver.

var rightExpression: NSExpression

The right expression for the receiver.

var leftExpression: NSExpression

The left expression for the receiver.

var options: NSComparisonPredicate.Options

The options to use for the receiver.

var predicateOperatorType: NSComparisonPredicate.Operator

The predicate type for the receiver.

enum Operator

Defines the type of comparison for a comparison predicate.

