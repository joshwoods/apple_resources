

- Foundation
-  PredicateExpression 

Protocol

# PredicateExpression

A component expression that makes up part of a predicate.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol PredicateExpression
```

## Overview

To transform a predicate, define a protocol for the result and add conformance on each predicate expression type that you support. For example:

```
protocol ProsePredicateExpression {
    func proseQuery() -> String
}

// Repeated for each supported operator.
extension PredicateExpressions.Equal: ProsePredicateExpression 
        where LHS: ProsePredicateExpression,
        RHS: ProsePredicateExpression {
    func proseQuery() -> String {
        return lhs.proseQuery() + " is equal to " + rhs.proseQuery()
    }
}

extension Predicate  {
    func proseQuery() -> String? {
        guard let expression = expression as? ProsePredicateExpression else { return nil }
        return expression.proseQuery()
    }
}
```

## Topics

### Evaluating a predicate expression

associatedtype Output

**Required**

func evaluate(PredicateBindings) throws -> Self.Output

**Required**

## Relationships

### Inherited By

- StandardPredicateExpression

### Conforming Types

- PredicateExpressions.Arithmetic
- PredicateExpressions.ClosedRange
- PredicateExpressions.CollectionContainsCollection
- PredicateExpressions.CollectionIndexSubscript

  Conforms when `Wrapped` conforms to `StandardPredicateExpression`, `Index` conforms to `StandardPredicateExpression`, `Wrapped.Output` conforms to `Collection`, and `Index.Output` is `Wrapped.Output.Index`.

- PredicateExpressions.CollectionRangeSubscript
- PredicateExpressions.Comparison
- PredicateExpressions.Conditional
- PredicateExpressions.ConditionalCast
- PredicateExpressions.Conjunction
- PredicateExpressions.DictionaryKeyDefaultValueSubscript
- PredicateExpressions.DictionaryKeySubscript
- PredicateExpressions.Disjunction

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` is `Bool`, and `RHS.Output` is `Bool`.

- PredicateExpressions.Equal
- PredicateExpressions.ExpressionEvaluate
- PredicateExpressions.Filter
- PredicateExpressions.FloatDivision
- PredicateExpressions.ForceCast
- PredicateExpressions.ForcedUnwrap
- PredicateExpressions.IntDivision

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `BinaryInteger`, and `LHS.Output` is `RHS.Output`.

- PredicateExpressions.IntRemainder

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `BinaryInteger`, and `LHS.Output` is `RHS.Output`.

- PredicateExpressions.KeyPath
- PredicateExpressions.Negation
- PredicateExpressions.NilCoalesce
- PredicateExpressions.NilLiteral
- PredicateExpressions.NotEqual
- PredicateExpressions.OptionalFlatMap
- PredicateExpressions.PredicateEvaluate
- PredicateExpressions.Range
- PredicateExpressions.RangeExpressionContains
- PredicateExpressions.SequenceAllSatisfy
- PredicateExpressions.SequenceContains
- PredicateExpressions.SequenceContainsWhere
- PredicateExpressions.SequenceMaximum
- PredicateExpressions.SequenceMinimum
- PredicateExpressions.SequenceStartsWith
- PredicateExpressions.StringCaseInsensitiveCompare
- PredicateExpressions.StringContainsRegex
- PredicateExpressions.StringLocalizedCompare
- PredicateExpressions.StringLocalizedStandardContains
- PredicateExpressions.TypeCheck
- PredicateExpressions.UnaryMinus
- PredicateExpressions.Value
- PredicateExpressions.Variable

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

