

- Foundation
-  PredicateError 

Structure

# PredicateError

An error thrown while evaluating a predicate.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct PredicateError
```

## Topics

### Errors

static let forceCastFailure: PredicateError

static let forceUnwrapFailure: PredicateError

static let invalidInput: PredicateError

static let undefinedVariable: PredicateError

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Filltering

struct Predicate

A logical condition used to test a set of input values for searching or filtering.

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

class NSCompoundPredicate

A specialized predicate that evaluates logical combinations of other predicates.

