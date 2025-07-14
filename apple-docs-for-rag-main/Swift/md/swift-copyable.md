

- Swift
-  Copyable 

Protocol

# Copyable

A type whose values can be implicitly or explicitly copied.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol Copyable
```

## Overview

Conforming to this protocol indicates that a type’s value can be copied; this protocol doesn’t have any required methods or properties. You don’t generally need to write an explicit conformance to `Copyable`. The following places implicitly include `Copyable` conformance:

- Structure declarations, unless it has a noncopyable stored property

- Enumeration declarations, unless it has a case whose associated value isn’t copyable

- Class declarations

- Actor declarations

- Protocol declarations

- Associated type declarations

- The `Self` type in a protocol extension

- In an extension, the generic parameters of the type being extended

A class or actor can contain noncopyable stored properties, while still being copyable itself — classes and actors are copied by retaining and releasing references.

In a declaration that includes generic type parameters, each generic type parameter implicitly includes `Copyable` in its list of requirements. Metatypes and tuples of copyable types are also implicitly copyable, as are boxed protocol types. For example, all of the following pairs of declarations are equivalent:

```
struct MyStructure { }
struct MyStructere: Copyable { }

protocol MyProtocol { }
protocol MyProtocol: Copyable { }

protocol AnotherProtocol {
    associatedtype MyType
    associatedtype MyType: Copyable
}

func genericFunction(t: T) { }
func genericFunction(t: T) where T: Copyable { }

let x: any MyProtocol
let x: any MyProtocol & Copyable
```

To suppress an implicit conformance to `Copyable` you write `~Copyable`. For example, only copyable types can conform to `MyProtocol` in the example above, but both copyable and noncopyable types can conform `NoRequirements` in the example below:

```
protocol NoRequirements: ~Copyable { }
```

Extensions to the `Copyable` protocol are not allowed.

## Relationships

### Conforming Types

- Anchor
- AnyBidirectionalCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AnyCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AnyHashable
- AnyIndex
- AnyIterator

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AnyKeyPath
- AnyRandomAccessCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AnyRegexOutput
- AnySequence

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Array

  Conforms when `Element` conforms to `Hashable`.

- ArraySlice

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AsyncCompactMapSequence

  Conforms when `Base` conforms to `AsyncSequence`, `ElementOfResult` conforms to `Copyable`, and `ElementOfResult` conforms to `Escapable`.

- AsyncDropFirstSequence

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncDropWhileSequence

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncFilterSequence

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncFlatMapSequence

  Conforms when `Base` conforms to `AsyncSequence` and `SegmentOfResult` conforms to `AsyncSequence`.

- AsyncMapSequence

  Conforms when `Base` conforms to `AsyncSequence`, `Transformed` conforms to `Copyable`, and `Transformed` conforms to `Escapable`.

- AsyncPrefixSequence

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncPrefixWhileSequence

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncStream

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AsyncStream.Continuation.Termination

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AsyncThrowingCompactMapSequence

  Conforms when `Base` conforms to `AsyncSequence`, `ElementOfResult` conforms to `Copyable`, and `ElementOfResult` conforms to `Escapable`.

- AsyncThrowingDropWhileSequence

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncThrowingFilterSequence

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncThrowingFlatMapSequence

  Conforms when `Base` conforms to `AsyncSequence` and `SegmentOfResult` conforms to `AsyncSequence`.

- AsyncThrowingMapSequence

  Conforms when `Base` conforms to `AsyncSequence`, `Transformed` conforms to `Copyable`, and `Transformed` conforms to `Escapable`.

- AsyncThrowingPrefixWhileSequence

  Conforms when `Base` conforms to `AsyncSequence`.

- AsyncThrowingStream

  Conforms when `Element` conforms to `Copyable`, `Element` conforms to `Escapable`, and `Failure` conforms to `Error`.

- AtomicLoadOrdering
- AtomicStoreOrdering
- AtomicUpdateOrdering
- AutoreleasingUnsafeMutablePointer

  Conforms when `Pointee` conforms to `Copyable` and `Escapable`.

- Bool
- CVaListPointer
- Capture

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- Character
- CharacterClass
- ChoiceOf

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- ClosedRange

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- ClosedRange.Index

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- CollectionDifference

  Conforms when `ChangeElement` conforms to `Equatable`.

- CollectionDifference.Change

  Conforms when `ChangeElement` conforms to `Equatable`.

- CollectionDifference.Index

  Conforms when `ChangeElement` conforms to `Copyable` and `Escapable`.

- CollectionOfOne

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- CollectionOfOne.Iterator

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousArray

  Conforms when `Element` conforms to `Hashable`.

- ContinuousClock
- ContinuousClock.Instant
- DecodingError
- DefaultIndices

  Conforms when `Elements` conforms to `Collection`.

- DefaultStringInterpolation
- Dictionary

  Conforms when `Key` conforms to `Decodable`, `Key` conforms to `Hashable`, and `Value` conforms to `Decodable`.

- Dictionary.Index

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Dictionary.Iterator

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Dictionary.Keys

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Dictionary.Values

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- DiscardingTaskGroup
- DiscontiguousSlice

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Hashable`.

- DiscontiguousSlice.Index

  Conforms when `Base` conforms to `Collection`.

- Double
- DropFirstSequence

  Conforms when `Base` conforms to `Sequence`.

- DropWhileSequence

  Conforms when `Base` conforms to `Sequence`.

- DropWhileSequence.Iterator

  Conforms when `Base` conforms to `Sequence`.

- Duration
- Duration.TimeFormatStyle
- Duration.TimeFormatStyle.Attributed
- Duration.UnitsFormatStyle
- Duration.UnitsFormatStyle.Attributed
- EmptyCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- EmptyCollection.Iterator

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- EncodingError
- EnumeratedSequence

  Conforms when `Base` conforms to `Sequence`.

- EnumeratedSequence.Iterator

  Conforms when `Base` conforms to `Sequence`.

- ExecuteDistributedTargetError.ErrorCode
- FlattenSequence

  Conforms when `Base` conforms to `Sequence` and `Base.Element` conforms to `Sequence`.

- FlattenSequence.Index

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Collection`.

- FlattenSequence.Iterator

  Conforms when `Base` conforms to `Sequence` and `Base.Element` conforms to `Sequence`.

- Float
- Float16
- Float80
- FloatingPointClassification
- FloatingPointRoundingRule
- FloatingPointSign
- Hasher
- IndexingIterator

  Conforms when `Elements` conforms to `Collection`.

- Int
- Int.Words
- Int128
- Int16
- Int16.Words
- Int32
- Int32.Words
- Int64
- Int64.Words
- Int8
- Int8.Words
- IteratorSequence

  Conforms when `Base` conforms to `IteratorProtocol`.

- JobPriority
- JoinedSequence

  Conforms when `Base` conforms to `Sequence` and `Base.Element` conforms to `Sequence`.

- JoinedSequence.Iterator

  Conforms when `Base` conforms to `Sequence` and `Base.Element` conforms to `Sequence`.

- KeyValuePairs

  Conforms when `Key` conforms to `Copyable`, `Key` conforms to `Escapable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- LazyDropWhileSequence

  Conforms when `Base` conforms to `Sequence`.

- LazyDropWhileSequence.Iterator

  Conforms when `Base` conforms to `Sequence`.

- LazyFilterSequence

  Conforms when `Base` conforms to `Collection`.

- LazyFilterSequence.Iterator

  Conforms when `Base` conforms to `Sequence`.

- LazyMapSequence

  Conforms when `Base` conforms to `Sequence`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- LazyMapSequence.Iterator

  Conforms when `Base` conforms to `Sequence`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- LazyPrefixWhileSequence

  Conforms when `Base` conforms to `BidirectionalCollection`.

- LazyPrefixWhileSequence.Index

  Conforms when `Base` conforms to `Collection` and `Base.Index` conforms to `Hashable`.

- LazyPrefixWhileSequence.Iterator

  Conforms when `Base` conforms to `Sequence`.

- LazySequence

  Conforms when `Base` conforms to `Sequence`.

- Local

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- Lookahead

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- ManagedBufferPointer

  Conforms when `Header` conforms to `Copyable`, `Header` conforms to `Escapable`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- Mirror
- Mirror.DisplayStyle
- NegativeLookahead

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- Never
- ObjectIdentifier
- ObservationRegistrar
- OneOrMore

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- OpaquePointer
- Optional

  Conforms when `Wrapped` conforms to `Copyable` and `Escapable`.

- Optional.Publisher

  Conforms when `Wrapped` conforms to `Equatable`.

- Optionally

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- PartialRangeFrom

  Conforms when `Bound` conforms to `Comparable` and `Encodable`.

- PartialRangeThrough

  Conforms when `Bound` conforms to `Comparable`.

- PartialRangeUpTo

  Conforms when `Bound` conforms to `Comparable` and `Encodable`.

- PrefixSequence

  Conforms when `Base` conforms to `Sequence`.

- PrefixSequence.Iterator

  Conforms when `Base` conforms to `Sequence`.

- Range

  Conforms when `Bound` conforms to `Comparable` and `Hashable`.

- RangeSet

  Conforms when `Bound` conforms to `Comparable` and `Hashable`.

- RangeSet.Ranges

  Conforms when `Bound` conforms to `Comparable` and `Hashable`.

- Repeat

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- Repeated

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Result

  Conforms when `Success` conforms to `Copyable`, `Success` conforms to `Escapable`, and `Failure` conforms to `Error`.

- Result.Publisher

  Conforms when `Success` conforms to `Equatable`, `Failure` conforms to `Equatable`, and `Failure` conforms to `Error`.

- ReversedCollection

  Conforms when `Base` conforms to `BidirectionalCollection` and `LazySequenceProtocol`.

- ReversedCollection.Index

  Conforms when `Base` conforms to `BidirectionalCollection` and `Base.Index` conforms to `Hashable`.

- ReversedCollection.Iterator

  Conforms when `Base` conforms to `BidirectionalCollection`.

- SIMD16

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD16Storage` conforms to `BitwiseCopyable`.

- SIMD2

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD2Storage` conforms to `BitwiseCopyable`.

- SIMD3

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD4Storage` conforms to `BitwiseCopyable`.

- SIMD32

  Conforms when `Scalar` conforms to `SIMDScalar`.

- SIMD4

  Conforms when `Scalar` conforms to `SIMDScalar`.

- SIMD64

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD64Storage` conforms to `BitwiseCopyable`.

- SIMD8

  Conforms when `Scalar` conforms to `SIMDScalar` and `Scalar.SIMD8Storage` conforms to `BitwiseCopyable`.

- Set

  Conforms when `Element` conforms to `Hashable`.

- Set.Index

  Conforms when `Element` conforms to `Hashable`.

- Set.Iterator

  Conforms when `Element` conforms to `Hashable`.

- Slice

  Conforms when `Base` conforms to `Collection`.

- StaticBigInt
- StaticString
- StrideThrough

  Conforms when `Element` conforms to `Strideable`.

- StrideThroughIterator

  Conforms when `Element` conforms to `Strideable`.

- StrideTo

  Conforms when `Element` conforms to `Strideable`.

- StrideToIterator

  Conforms when `Element` conforms to `Strideable`.

- String
- String.Encoding
- String.Index
- String.IntentInputOptions.CapitalizationType
- String.IntentInputOptions.KeyboardType
- String.LocalizationValue
- String.UTF16View
- String.UTF8View
- String.UnicodeScalarView
- Substring
- Substring.UTF16View
- Substring.UTF8View
- Substring.UnicodeScalarView
- SuspendingClock
- SuspendingClock.Instant
- SystemRandomNumberGenerator
- Task

  Conforms when `Success` conforms to `Copyable`, `Success` conforms to `Escapable`, `Success` conforms to `Sendable`, and `Failure` conforms to `Error`.

- TaskGroup

  Conforms when `ChildTaskResult` conforms to `Copyable`, `Escapable`, and `Sendable`.

- TaskPriority
- ThrowingDiscardingTaskGroup

  Conforms when `Failure` conforms to `Error`.

- ThrowingTaskGroup

  Conforms when `ChildTaskResult` conforms to `Copyable`, `ChildTaskResult` conforms to `Escapable`, `ChildTaskResult` conforms to `Sendable`, and `Failure` conforms to `Error`.

- TryCapture

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- UInt
- UInt.Words
- UInt128
- UInt128.Words
- UInt16
- UInt16.Words
- UInt32
- UInt32.Words
- UInt64
- UInt64.Words
- UInt8
- UInt8.Words
- UnboundedRange_
- Unicode.ASCII
- Unicode.ASCII.Parser
- Unicode.GeneralCategory
- Unicode.NumericType
- Unicode.Scalar
- Unicode.Scalar.UTF16View
- Unicode.Scalar.UTF8View
- Unicode.UTF16
- Unicode.UTF16.ForwardParser
- Unicode.UTF16.ReverseParser
- Unicode.UTF32
- Unicode.UTF32.Parser
- Unicode.UTF8
- Unicode.UTF8.ForwardParser
- Unicode.UTF8.ReverseParser
- UnicodeDecodingResult
- Unmanaged

  Conforms when `Instance` conforms to `Copyable` and `Escapable`.

- UnownedJob
- UnownedSerialExecutor
- UnownedTaskExecutor
- UnsafeBufferPointer

  Conforms when `Element` conforms to `Escapable`.

- UnsafeBufferPointer.Iterator

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- UnsafeContinuation

  Conforms when `T` conforms to `Copyable`, `T` conforms to `Escapable`, and `E` conforms to `Error`.

- UnsafeCurrentTask
- UnsafeMutableBufferPointer

  Conforms when `Element` conforms to `Escapable`.

- UnsafeMutablePointer

  Conforms when `Pointee` conforms to `Escapable`.

- UnsafeMutableRawBufferPointer
- UnsafeMutableRawPointer
- UnsafePointer

  Conforms when `Pointee` conforms to `Copyable` and `Escapable`.

- UnsafeRawBufferPointer
- UnsafeRawBufferPointer.Iterator
- UnsafeRawPointer
- WordPair
- ZeroOrMore

  Conforms when `Output` conforms to `Copyable` and `Escapable`.

- Zip2Sequence

  Conforms when `Sequence1` conforms to `Sequence` and `Sequence2` conforms to `Sequence`.

- Zip2Sequence.Iterator

  Conforms when `Sequence1` conforms to `Sequence` and `Sequence2` conforms to `Sequence`.

## See Also

### Copying

protocol BitwiseCopyable

