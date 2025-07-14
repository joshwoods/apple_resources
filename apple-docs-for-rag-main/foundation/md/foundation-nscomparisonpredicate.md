

- Foundation
-  NSComparisonPredicate 

Class

# NSComparisonPredicate

A specialized predicate for comparing expressions.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSComparisonPredicate
```

## Overview

Use comparison predicates to compare the results of two expressions. You create a comparison predicate with an operator, a left expression, and a right expression, and use instances of the NSExpression class to represent those expressions. When you evaluate the predicate, it returns a `BOOL` value as the result of invoking the operator with the results of evaluating the expressions.

## Topics

### Creating Comparison Predicates

Displaying searchable content by using a search controller

Create a user interface with searchable content in a table view.

init(leftExpression: NSExpression, rightExpression: NSExpression, customSelector: Selector)

Creates a predicate that you form by combining specified left and right expressions using a specified selector.

init(leftExpression: NSExpression, rightExpression: NSExpression, modifier: NSComparisonPredicate.Modifier, type: NSComparisonPredicate.Operator, options: NSComparisonPredicate.Options)

Creates a predicate to a specified type that you form by combining specified left and right expressions using a specified modifier and options.

init?(coder: NSCoder)

Creates a predicate by decoding from the coder you specify.

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

struct Options

Constants that describe the possible types of string comparison for comparison predicates.

var predicateOperatorType: NSComparisonPredicate.Operator

The predicate type for the receiver.

enum Operator

Defines the type of comparison for a comparison predicate.

## Relationships

### Inherits From

- NSPredicate

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Filltering

struct Predicate

A logical condition used to test a set of input values for searching or filtering.

struct PredicateError

An error thrown while evaluating a predicate.

struct PredicateCodableConfiguration

A specification of the expected types and key paths found in an archived predicate.

protocol PredicateCodableKeyPathProviding

A type that provides the expected key paths found in an archived predicate.

protocol PredicateExpression

A component expression that makes up part of a predicate.

protocol StandardPredicateExpression

A component expression that makes up part of a predicate, and that’s supported by the standard predicate type.

enum PredicateExpressions

The expressions that make up a predicate.

struct PredicateBindings

A mapping from a predicates’s input variables to their values.

class NSPredicate

A definition of logical conditions for constraining a search for a fetch or for in-memory filtering.

class NSExpression

An expression for use in a comparison predicate.

class NSCompoundPredicate

A specialized predicate that evaluates logical combinations of other predicates.

