

- Foundation
-  NSCompoundPredicate 

Class

# NSCompoundPredicate

A specialized predicate that evaluates logical combinations of other predicates.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSCompoundPredicate
```

## Overview

Use NSCompoundPredicate to create an `AND` or `OR` compound predicate of one or more other predicates, or the `NOT` of a single predicate. For the logical `AND` and `OR` operations:

- An `AND` predicate with no subpredicates evaluates to true.

- An `OR` predicate with no subpredicates evaluates to false.

- A compound predicate with one or more subpredicates evaluates to the truth of its subpredicates.

## Topics

### Creating Compound Predicates

init(andPredicateWithSubpredicates: [NSPredicate])

Returns a new predicate that you form using an AND operation on the predicates in a specified array.

init(notPredicateWithSubpredicate: NSPredicate)

Returns a new predicate that you form using a NOT operation on a specified predicate.

init(orPredicateWithSubpredicates: [NSPredicate])

Returns a new predicate that you form using an OR operation on the predicates in a specified array.

init(type: NSCompoundPredicate.LogicalType, subpredicates: [NSPredicate])

Returns the receiver that a specified type initializes using predicates from a specified array.

init?(coder: NSCoder)

Creates a predicate by decoding from the coder you specify.

### Getting Information About a Compound Predicate

var compoundPredicateType: NSCompoundPredicate.LogicalType

The predicate type for the receiver.

var subpredicates: [Any]

The receiver’s subpredicates.

enum LogicalType

Constants that describe the possible types of a compound predicate.

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

class NSComparisonPredicate

A specialized predicate for comparing expressions.

