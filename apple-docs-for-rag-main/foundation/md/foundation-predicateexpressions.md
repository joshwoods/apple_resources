

- Foundation
-  PredicateExpressions 

Enumeration

# PredicateExpressions

The expressions that make up a predicate.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
enum PredicateExpressions
```

## Overview

Don’t use this type directly. When you call the `Predicate(_:)` macro in your code, the expansion of that macro produces these values.

## Topics

### Structures

struct Arithmetic

struct ClosedRange

struct CollectionContainsCollection

struct CollectionIndexSubscript

struct CollectionRangeSubscript

struct Comparison

struct Conditional

struct ConditionalCast

struct Conjunction

struct DictionaryKeyDefaultValueSubscript

struct DictionaryKeySubscript

struct Disjunction

struct Equal

struct ExpressionEvaluate

struct Filter

struct FloatDivision

struct ForceCast

struct ForcedUnwrap

struct IntDivision

struct IntRemainder

struct KeyPath

struct Negation

struct NilCoalesce

struct NilLiteral

struct NotEqual

struct OptionalFlatMap

struct PredicateEvaluate

struct PredicateRegex

struct Range

struct RangeExpressionContains

struct SequenceAllSatisfy

struct SequenceContains

struct SequenceContainsWhere

struct SequenceMaximum

struct SequenceMinimum

struct SequenceStartsWith

struct StringCaseInsensitiveCompare

struct StringContainsRegex

struct StringLocalizedCompare

struct StringLocalizedStandardContains

struct TypeCheck

struct UnaryMinus

struct Value

struct Variable

struct VariableID

### Type Methods

static func build_Arg&lt;T>(T) -> PredicateExpressions.Value&lt;T>

static func build_Arg&lt;T>(T) -> T

static func build_Arg(some RegexComponent) -> PredicateExpressions.Value&lt;PredicateExpressions.PredicateRegex>

static func build_Arithmetic&lt;LHS, RHS>(lhs: LHS, rhs: RHS, op: PredicateExpressions.ArithmeticOperator) -> PredicateExpressions.Arithmetic&lt;LHS, RHS>

static func build_ClosedRange&lt;LHS, RHS>(lower: LHS, upper: RHS) -> PredicateExpressions.ClosedRange&lt;LHS, RHS>

static func build_Comparison&lt;LHS, RHS>(lhs: LHS, rhs: RHS, op: PredicateExpressions.ComparisonOperator) -> PredicateExpressions.Comparison&lt;LHS, RHS>

static func build_Conditional&lt;Test, If, Else>(Test, If, Else) -> PredicateExpressions.Conditional&lt;Test, If, Else>

static func build_Conjunction&lt;LHS, RHS>(lhs: LHS, rhs: RHS) -> PredicateExpressions.Conjunction&lt;LHS, RHS>

static func build_Disjunction&lt;LHS, RHS>(lhs: LHS, rhs: RHS) -> PredicateExpressions.Disjunction&lt;LHS, RHS>

static func build_Division&lt;LHS, RHS>(lhs: LHS, rhs: RHS) -> PredicateExpressions.FloatDivision&lt;LHS, RHS>

static func build_Division&lt;LHS, RHS>(lhs: LHS, rhs: RHS) -> PredicateExpressions.IntDivision&lt;LHS, RHS>

static func build_Equal&lt;LHS, RHS>(lhs: LHS, rhs: RHS) -> PredicateExpressions.Equal&lt;LHS, RHS>

static func build_ForcedUnwrap&lt;Inner, Wrapped>(Inner) -> PredicateExpressions.ForcedUnwrap&lt;Inner, Wrapped>

static func build_KeyPath&lt;Root, Value>(root: Root, keyPath: any KeyPath&lt;Root.Output, Value> &amp; Sendable) -> PredicateExpressions.KeyPath&lt;Root, Value>

static func build_Negation&lt;T>(T) -> PredicateExpressions.Negation&lt;T>

static func build_NilCoalesce&lt;LHS, RHS>(lhs: LHS, rhs: RHS) -> PredicateExpressions.NilCoalesce&lt;LHS, RHS>

static func build_NilLiteral&lt;Wrapped>() -> PredicateExpressions.NilLiteral&lt;Wrapped>

static func build_NotEqual&lt;LHS, RHS>(lhs: LHS, rhs: RHS) -> PredicateExpressions.NotEqual&lt;LHS, RHS>

static func build_Range&lt;LHS, RHS>(lower: LHS, upper: RHS) -> PredicateExpressions.Range&lt;LHS, RHS>

static func build_Remainder&lt;LHS, RHS>(lhs: LHS, rhs: RHS) -> PredicateExpressions.IntRemainder&lt;LHS, RHS>

static func build_UnaryMinus&lt;T>(T) -> PredicateExpressions.UnaryMinus&lt;T>

static func build_allSatisfy&lt;LHS, RHS>(LHS, (PredicateExpressions.Variable&lt;LHS.Output.Element>) -> RHS) -> PredicateExpressions.SequenceAllSatisfy&lt;LHS, RHS>

static func build_caseInsensitiveCompare&lt;Root, Other>(Root, Other) -> PredicateExpressions.StringCaseInsensitiveCompare&lt;Root, Other>

static func build_contains&lt;Base, Other>(Base, Other) -> PredicateExpressions.CollectionContainsCollection&lt;Base, Other>

static func build_contains&lt;LHS, RHS>(LHS, RHS) -> PredicateExpressions.SequenceContains&lt;LHS, RHS>

static func build_contains&lt;Subject, Regex>(Subject, Regex) -> PredicateExpressions.StringContainsRegex&lt;Subject, Regex>

static func build_contains&lt;RangeExpression, Element>(RangeExpression, Element) -> PredicateExpressions.RangeExpressionContains&lt;RangeExpression, Element>

static func build_contains&lt;LHS, RHS>(LHS, where: (PredicateExpressions.Variable&lt;LHS.Output.Element>) -> RHS) -> PredicateExpressions.SequenceContainsWhere&lt;LHS, RHS>

static func build_evaluate&lt;Transformation, each Input, Output>(Transformation, repeat each Input) -> PredicateExpressions.ExpressionEvaluate&lt;Transformation, repeat each Input, Output>

static func build_evaluate&lt;Condition, each Input>(Condition, repeat each Input) -> PredicateExpressions.PredicateEvaluate&lt;Condition, repeat each Input>

static func build_filter&lt;LHS, RHS>(LHS, (PredicateExpressions.Variable&lt;LHS.Output.Element>) -> RHS) -> PredicateExpressions.Filter&lt;LHS, RHS>

static func build_flatMap&lt;LHS, RHS, Wrapped, Result>(LHS, (PredicateExpressions.Variable&lt;Wrapped>) -> RHS) -> PredicateExpressions.OptionalFlatMap&lt;LHS, Wrapped, RHS, Result>

static func build_flatMap&lt;LHS, RHS, Wrapped, Result>(LHS, (PredicateExpressions.Variable&lt;Wrapped>) -> RHS) -> PredicateExpressions.OptionalFlatMap&lt;LHS, Wrapped, RHS, Result>

static func build_localizedCompare&lt;Root, Other>(Root, Other) -> PredicateExpressions.StringLocalizedCompare&lt;Root, Other>

static func build_localizedStandardContains&lt;Root, Other>(Root, Other) -> PredicateExpressions.StringLocalizedStandardContains&lt;Root, Other>

static func build_max&lt;Elements>(Elements) -> PredicateExpressions.SequenceMaximum&lt;Elements>

static func build_min&lt;Elements>(Elements) -> PredicateExpressions.SequenceMinimum&lt;Elements>

static func build_starts&lt;Base, Prefix>(Base, with: Prefix) -> PredicateExpressions.SequenceStartsWith&lt;Base, Prefix>

static func build_subscript&lt;Wrapped, Key, Value>(Wrapped, Key) -> PredicateExpressions.DictionaryKeySubscript&lt;Wrapped, Key, Value>

static func build_subscript&lt;Wrapped, Range>(Wrapped, Range) -> PredicateExpressions.CollectionRangeSubscript&lt;Wrapped, Range>

static func build_subscript&lt;Wrapped, Index>(Wrapped, Index) -> PredicateExpressions.CollectionIndexSubscript&lt;Wrapped, Index>

static func build_subscript&lt;Wrapped, Key, Default>(Wrapped, Key, default: Default) -> PredicateExpressions.DictionaryKeyDefaultValueSubscript&lt;Wrapped, Key, Default>

### Enumerations

enum ArithmeticOperator

enum ComparisonOperator

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable

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

