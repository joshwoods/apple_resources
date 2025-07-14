

- Foundation
-  StandardPredicateExpression 

Protocol

# StandardPredicateExpression

A component expression that makes up part of a predicate, and that’s supported by the standard predicate type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol StandardPredicateExpression : PredicateExpression, Decodable, Encodable, Sendable
```

## Overview

Don’t declare new types that conform to the `StandardPredicateExpression` protocol. Only the types provided by Foundation are valid conforming types.

## Relationships

### Inherits From

- Decodable
- Encodable
- PredicateExpression
- Sendable

### Conforming Types

- PredicateExpressions.Arithmetic

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Numeric`, and `LHS.Output` is `RHS.Output`.

- PredicateExpressions.ClosedRange

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Comparable`, and `LHS.Output` is `RHS.Output`.

- PredicateExpressions.CollectionContainsCollection

  Conforms when `Base` conforms to `StandardPredicateExpression`, `Other` conforms to `StandardPredicateExpression`, `Base.Output` conforms to `Collection`, `Other.Output` conforms to `Collection`, `Base.Output.Element` conforms to `Equatable`, and `Base.Output.Element` is `Other.Output.Element`.

- PredicateExpressions.CollectionIndexSubscript

  Conforms when `Wrapped` conforms to `StandardPredicateExpression`, `Index` conforms to `StandardPredicateExpression`, `Wrapped.Output` conforms to `Collection`, and `Index.Output` is `Wrapped.Output.Index`.

- PredicateExpressions.CollectionRangeSubscript

  Conforms when `Wrapped` conforms to `StandardPredicateExpression`, `Range` conforms to `StandardPredicateExpression`, `Wrapped.Output` conforms to `Collection`, and `Range.Output` is `Range`.

- PredicateExpressions.Comparison

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Comparable`, and `LHS.Output` is `RHS.Output`.

- PredicateExpressions.Conditional

  Conforms when `Test` conforms to `StandardPredicateExpression`, `If` conforms to `StandardPredicateExpression`, `Else` conforms to `StandardPredicateExpression`, `Test.Output` is `Bool`, and `If.Output` is `Else.Output`.

- PredicateExpressions.ConditionalCast

  Conforms when `Input` conforms to `StandardPredicateExpression`, `Desired` conforms to `Copyable`, and `Desired` conforms to `Escapable`.

- PredicateExpressions.Conjunction

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` is `Bool`, and `RHS.Output` is `Bool`.

- PredicateExpressions.DictionaryKeyDefaultValueSubscript

  Conforms when `Wrapped` conforms to `StandardPredicateExpression`, `Key` conforms to `StandardPredicateExpression`, `Default` conforms to `StandardPredicateExpression`, `Wrapped.Output` is `[Key.Output : Default.Output]`, and `Key.Output` conforms to `Hashable`.

- PredicateExpressions.DictionaryKeySubscript

  Conforms when `Wrapped` conforms to `StandardPredicateExpression`, `Key` conforms to `StandardPredicateExpression`, `Value` conforms to `Copyable`, `Value` conforms to `Escapable`, `Wrapped.Output` is `[Key.Output : Value]`, and `Key.Output` conforms to `Hashable`.

- PredicateExpressions.Disjunction

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` is `Bool`, and `RHS.Output` is `Bool`.

- PredicateExpressions.Equal

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Equatable`, and `LHS.Output` is `RHS.Output`.

- PredicateExpressions.ExpressionEvaluate

  Conforms when `Transformation` conforms to `StandardPredicateExpression`, `each Input` conforms to `StandardPredicateExpression`, `Output` conforms to `Copyable`, `Output` conforms to `Escapable`, and `Transformation.Output` is `Expression`.

- PredicateExpressions.Filter

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Sequence`, and `RHS.Output` is `Bool`.

- PredicateExpressions.FloatDivision

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `FloatingPoint`, and `LHS.Output` is `RHS.Output`.

- PredicateExpressions.ForceCast

  Conforms when `Input` conforms to `StandardPredicateExpression`, `Desired` conforms to `Copyable`, and `Desired` conforms to `Escapable`.

- PredicateExpressions.ForcedUnwrap

  Conforms when `Inner` conforms to `StandardPredicateExpression`, `Wrapped` conforms to `Copyable`, `Wrapped` conforms to `Escapable`, and `Inner.Output` is `Wrapped?`.

- PredicateExpressions.IntDivision

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `BinaryInteger`, and `LHS.Output` is `RHS.Output`.

- PredicateExpressions.IntRemainder

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `BinaryInteger`, and `LHS.Output` is `RHS.Output`.

- PredicateExpressions.KeyPath

  Conforms when `Root` conforms to `StandardPredicateExpression`, `Output` conforms to `Copyable`, and `Output` conforms to `Escapable`.

- PredicateExpressions.Negation

  Conforms when `Wrapped` conforms to `StandardPredicateExpression` and `Wrapped.Output` is `Bool`.

- PredicateExpressions.NilCoalesce

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, and `LHS.Output` is `RHS.Output?`.

- PredicateExpressions.NilLiteral
- PredicateExpressions.NotEqual

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Equatable`, and `LHS.Output` is `RHS.Output`.

- PredicateExpressions.OptionalFlatMap

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `Wrapped` conforms to `Copyable`, `Wrapped` conforms to `Escapable`, `RHS` conforms to `StandardPredicateExpression`, `Result` conforms to `Copyable`, `Result` conforms to `Escapable`, and `LHS.Output` is `Wrapped?`.

- PredicateExpressions.PredicateEvaluate

  Conforms when `Condition` conforms to `StandardPredicateExpression`, `each Input` conforms to `StandardPredicateExpression`, and `Condition.Output` is `Predicate`.

- PredicateExpressions.Range

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Comparable`, and `LHS.Output` is `RHS.Output`.

- PredicateExpressions.RangeExpressionContains

  Conforms when `RangeExpression` conforms to `StandardPredicateExpression`, `Element` conforms to `StandardPredicateExpression`, `RangeExpression.Output` conforms to `RangeExpression`, and `Element.Output` is `RangeExpression.Output.Bound`.

- PredicateExpressions.SequenceAllSatisfy

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Sequence`, and `RHS.Output` is `Bool`.

- PredicateExpressions.SequenceContains

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Sequence`, `RHS.Output` conforms to `Equatable`, and `RHS.Output` is `LHS.Output.Element`.

- PredicateExpressions.SequenceContainsWhere

  Conforms when `LHS` conforms to `StandardPredicateExpression`, `RHS` conforms to `StandardPredicateExpression`, `LHS.Output` conforms to `Sequence`, and `RHS.Output` is `Bool`.

- PredicateExpressions.SequenceMaximum

  Conforms when `Elements` conforms to `StandardPredicateExpression`, `Elements.Output` conforms to `Sequence`, and `Elements.Output.Element` conforms to `Comparable`.

- PredicateExpressions.SequenceMinimum

  Conforms when `Elements` conforms to `StandardPredicateExpression`, `Elements.Output` conforms to `Sequence`, and `Elements.Output.Element` conforms to `Comparable`.

- PredicateExpressions.SequenceStartsWith

  Conforms when `Base` conforms to `StandardPredicateExpression`, `Prefix` conforms to `StandardPredicateExpression`, `Base.Output` conforms to `Sequence`, `Prefix.Output` conforms to `Sequence`, `Base.Output.Element` conforms to `Equatable`, and `Base.Output.Element` is `Prefix.Output.Element`.

- PredicateExpressions.StringCaseInsensitiveCompare

  Conforms when `Root` conforms to `StandardPredicateExpression`, `Other` conforms to `StandardPredicateExpression`, `Root.Output` conforms to `StringProtocol`, and `Other.Output` conforms to `StringProtocol`.

- PredicateExpressions.StringContainsRegex

  Conforms when `Subject` conforms to `StandardPredicateExpression`, `Regex` conforms to `StandardPredicateExpression`, `Subject.Output` conforms to `BidirectionalCollection`, `Regex.Output` conforms to `RegexComponent`, and `Subject.Output.SubSequence` is `Substring`.

- PredicateExpressions.StringLocalizedCompare

  Conforms when `Root` conforms to `StandardPredicateExpression`, `Other` conforms to `StandardPredicateExpression`, `Root.Output` conforms to `StringProtocol`, and `Other.Output` conforms to `StringProtocol`.

- PredicateExpressions.StringLocalizedStandardContains

  Conforms when `Root` conforms to `StandardPredicateExpression`, `Other` conforms to `StandardPredicateExpression`, `Root.Output` conforms to `StringProtocol`, and `Other.Output` conforms to `StringProtocol`.

- PredicateExpressions.TypeCheck

  Conforms when `Input` conforms to `StandardPredicateExpression`, `Desired` conforms to `Copyable`, and `Desired` conforms to `Escapable`.

- PredicateExpressions.UnaryMinus

  Conforms when `Wrapped` conforms to `StandardPredicateExpression` and `Wrapped.Output` conforms to `SignedNumeric`.

- PredicateExpressions.Value

  Conforms when `Output` conforms to `Decodable` and `Encodable`.

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

protocol PredicateExpression

A component expression that makes up part of a predicate.

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

