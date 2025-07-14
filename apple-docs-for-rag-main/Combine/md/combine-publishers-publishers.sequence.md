

- Combine
- Publishers
-  Publishers.Sequence 

Structure

# Publishers.Sequence

A publisher that publishes a given sequence of elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Sequence where Elements : Sequence, Failure : Error
```

## Overview

When the publisher exhausts the elements in the sequence, the next request causes the publisher to finish.

## Topics

### Creating a Sequence Publisher

init(sequence: Elements)

Creates a publisher for a sequence of elements.

### Declaring Publisher Topography

typealias Output

The kind of values published by this publisher.

### Inspecting Publisher Properties

let sequence: Elements

The sequence of elements to publish.

### Comparing Publishers

static func == (Publishers.Sequence&lt;Elements, Failure>, Publishers.Sequence&lt;Elements, Failure>) -> Bool

Returns a Boolean value that indicates whether two publishers are equivalent.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Applying Operators

Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

### Instance Methods

func allSatisfy((Publishers.Sequence&lt;Elements, Failure>.Output) -> Bool) -> Result&lt;Bool, Failure>.Publisher

func append(Publishers.Sequence&lt;Elements, Failure>.Output...) -> Publishers.Sequence&lt;Elements, Failure>

func append(Publishers.Sequence&lt;Elements, Failure>) -> Publishers.Sequence&lt;Elements, Failure>

func append&lt;S>(S) -> Publishers.Sequence&lt;Elements, Failure>

func collect() -> Result&lt;[Publishers.Sequence&lt;Elements, Failure>.Output], Failure>.Publisher

func compactMap&lt;T>((Publishers.Sequence&lt;Elements, Failure>.Output) -> T?) -> Publishers.Sequence&lt;[T], Failure>

func contains(Elements.Element) -> Result&lt;Bool, Failure>.Publisher

func contains(where: (Publishers.Sequence&lt;Elements, Failure>.Output) -> Bool) -> Result&lt;Bool, Failure>.Publisher

func count() -> Result&lt;Int, Failure>.Publisher

func count() -> Just&lt;Int>

func count() -> Result&lt;Int, Failure>.Publisher

func drop(while: (Elements.Element) -> Bool) -> Publishers.Sequence&lt;DropWhileSequence&lt;Elements>, Failure>

func dropFirst(Int) -> Publishers.Sequence&lt;DropFirstSequence&lt;Elements>, Failure>

func filter((Publishers.Sequence&lt;Elements, Failure>.Output) -> Bool) -> Publishers.Sequence&lt;[Publishers.Sequence&lt;Elements, Failure>.Output], Failure>

func first() -> Optional&lt;Publishers.Sequence&lt;Elements, Failure>.Output>.Publisher

func first(where: (Publishers.Sequence&lt;Elements, Failure>.Output) -> Bool) -> Optional&lt;Publishers.Sequence&lt;Elements, Failure>.Output>.Publisher

func ignoreOutput() -> Empty&lt;Publishers.Sequence&lt;Elements, Failure>.Output, Failure>

func last() -> Optional&lt;Publishers.Sequence&lt;Elements, Failure>.Output>.Publisher

func last(where: (Publishers.Sequence&lt;Elements, Failure>.Output) -> Bool) -> Optional&lt;Publishers.Sequence&lt;Elements, Failure>.Output>.Publisher

func map&lt;T>((Elements.Element) -> T) -> Publishers.Sequence&lt;[T], Failure>

func max() -> Optional&lt;Publishers.Sequence&lt;Elements, Failure>.Output>.Publisher

func max(by: (Publishers.Sequence&lt;Elements, Failure>.Output, Publishers.Sequence&lt;Elements, Failure>.Output) -> Bool) -> Optional&lt;Publishers.Sequence&lt;Elements, Failure>.Output>.Publisher

func min() -> Optional&lt;Publishers.Sequence&lt;Elements, Failure>.Output>.Publisher

func min(by: (Publishers.Sequence&lt;Elements, Failure>.Output, Publishers.Sequence&lt;Elements, Failure>.Output) -> Bool) -> Optional&lt;Publishers.Sequence&lt;Elements, Failure>.Output>.Publisher

func output(at: Elements.Index) -> Optional&lt;Publishers.Sequence&lt;Elements, Failure>.Output>.Publisher

func output(at: Elements.Index) -> Optional&lt;Publishers.Sequence&lt;Elements, Failure>.Output>.Publisher

func output(in: Range&lt;Elements.Index>) -> Publishers.Sequence&lt;[Publishers.Sequence&lt;Elements, Failure>.Output], Failure>

func output(in: Range&lt;Elements.Index>) -> Publishers.Sequence&lt;[Publishers.Sequence&lt;Elements, Failure>.Output], Failure>

func prefix(Int) -> Publishers.Sequence&lt;PrefixSequence&lt;Elements>, Failure>

func prefix(while: (Elements.Element) -> Bool) -> Publishers.Sequence&lt;[Elements.Element], Failure>

func prepend&lt;S>(S) -> Publishers.Sequence&lt;Elements, Failure>

func prepend(Publishers.Sequence&lt;Elements, Failure>.Output...) -> Publishers.Sequence&lt;Elements, Failure>

func prepend(Publishers.Sequence&lt;Elements, Failure>) -> Publishers.Sequence&lt;Elements, Failure>

func reduce&lt;T>(T, (T, Publishers.Sequence&lt;Elements, Failure>.Output) -> T) -> Result&lt;T, Failure>.Publisher

func removeDuplicates() -> Publishers.Sequence&lt;[Publishers.Sequence&lt;Elements, Failure>.Output], Failure>

func replaceNil&lt;T>(with: T) -> Publishers.Sequence&lt;[Publishers.Sequence&lt;Elements, Failure>.Output], Failure>

func scan&lt;T>(T, (T, Publishers.Sequence&lt;Elements, Failure>.Output) -> T) -> Publishers.Sequence&lt;[T], Failure>

func setFailureType&lt;E>(to: E.Type) -> Publishers.Sequence&lt;Elements, E>

func tryAllSatisfy((Publishers.Sequence&lt;Elements, Failure>.Output) throws -> Bool) -> Result&lt;Bool, any Error>.Publisher

func tryContains(where: (Publishers.Sequence&lt;Elements, Failure>.Output) throws -> Bool) -> Result&lt;Bool, any Error>.Publisher

func tryReduce&lt;T>(T, (T, Publishers.Sequence&lt;Elements, Failure>.Output) throws -> T) -> Result&lt;T, any Error>.Publisher

### Default Implementations

Equatable Implementations

Publisher Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Publisher

## See Also

### Convenience Publishers

struct Catch

A publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher.

