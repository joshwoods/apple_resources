

- Swift
- Optional
-  Optional.Publisher 

Structure

# Optional.Publisher

The type of a Combine publisher that publishes the value of a Swift optional instance to each subscriber exactly once, if the instance has any value at all.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Publisher
```

## Overview

In contrast with the Just publisher, which always produces a single value, this publisher might not send any values and instead finish normally, if output is `nil`.

## Topics

### Declaring Publisher Topography

typealias Output

The kind of value published by this publisher.

typealias Failure

The kind of error this publisher might publish.

### Creating an Optional Publisher

init(Optional&lt;Wrapped>.Publisher.Output?)

Creates a publisher to emit the value of the optional, or to finish immediately if the optional doesn’t have a value.

### Inpsecting Publisher Properties

let output: Optional&lt;Wrapped>.Publisher.Output?

The output to deliver to each subscriber.

### Working with Subscribers

func receive&lt;S>(subscriber: S)

Implements the Publisher protocol by accepting the subscriber and immediately publishing the optional’s value if it has one, or finishing normally if it doesn’t.

### Instance Methods

func allSatisfy((Optional&lt;Wrapped>.Publisher.Output) -> Bool) -> Optional&lt;Bool>.Publisher

func collect() -> Optional&lt;[Optional&lt;Wrapped>.Publisher.Output]>.Publisher

func compactMap&lt;T>((Optional&lt;Wrapped>.Publisher.Output) -> T?) -> Optional&lt;T>.Publisher

func contains(Optional&lt;Wrapped>.Publisher.Output) -> Optional&lt;Bool>.Publisher

func contains(where: (Optional&lt;Wrapped>.Publisher.Output) -> Bool) -> Optional&lt;Bool>.Publisher

func count() -> Optional&lt;Int>.Publisher

func drop(while: (Optional&lt;Wrapped>.Publisher.Output) -> Bool) -> Optional&lt;Wrapped>.Publisher

func dropFirst(Int) -> Optional&lt;Wrapped>.Publisher

func filter((Optional&lt;Wrapped>.Publisher.Output) -> Bool) -> Optional&lt;Wrapped>.Publisher

func first() -> Optional&lt;Wrapped>.Publisher

func first(where: (Optional&lt;Wrapped>.Publisher.Output) -> Bool) -> Optional&lt;Wrapped>.Publisher

func ignoreOutput() -> Empty&lt;Optional&lt;Wrapped>.Publisher.Output, Optional&lt;Wrapped>.Publisher.Failure>

func last() -> Optional&lt;Wrapped>.Publisher

func last(where: (Optional&lt;Wrapped>.Publisher.Output) -> Bool) -> Optional&lt;Wrapped>.Publisher

func map&lt;T>((Optional&lt;Wrapped>.Publisher.Output) -> T) -> Optional&lt;T>.Publisher

func max() -> Optional&lt;Wrapped>.Publisher

func max(by: (Optional&lt;Wrapped>.Publisher.Output, Optional&lt;Wrapped>.Publisher.Output) -> Bool) -> Optional&lt;Wrapped>.Publisher

func min() -> Optional&lt;Wrapped>.Publisher

func min(by: (Optional&lt;Wrapped>.Publisher.Output, Optional&lt;Wrapped>.Publisher.Output) -> Bool) -> Optional&lt;Wrapped>.Publisher

func output(at: Int) -> Optional&lt;Wrapped>.Publisher

func output&lt;R>(in: R) -> Optional&lt;Wrapped>.Publisher

func prefix(Int) -> Optional&lt;Wrapped>.Publisher

func prefix(while: (Optional&lt;Wrapped>.Publisher.Output) -> Bool) -> Optional&lt;Wrapped>.Publisher

func reduce&lt;T>(T, (T, Optional&lt;Wrapped>.Publisher.Output) -> T) -> Optional&lt;T>.Publisher

func removeDuplicates() -> Optional&lt;Wrapped>.Publisher

func removeDuplicates(by: (Optional&lt;Wrapped>.Publisher.Output, Optional&lt;Wrapped>.Publisher.Output) -> Bool) -> Optional&lt;Wrapped>.Publisher

func replaceEmpty(with: Optional&lt;Wrapped>.Publisher.Output) -> Just&lt;Wrapped>

func replaceError(with: Optional&lt;Wrapped>.Publisher.Output) -> Optional&lt;Optional&lt;Wrapped>.Publisher.Output>.Publisher

func retry(Int) -> Optional&lt;Wrapped>.Publisher

func scan&lt;T>(T, (T, Optional&lt;Wrapped>.Publisher.Output) -> T) -> Optional&lt;T>.Publisher

### Default Implementations

Equatable Implementations

Publisher Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Wrapped` conforms to `Equatable`.

- Equatable

  Conforms when `Wrapped` conforms to `Equatable`.

- Publisher

## See Also

### Publishing an Optional

var publisher: Optional&lt;Wrapped>.Publisher

A Combine publisher that publishes this instance’s value to each subscriber exactly once, if it has any value at all.

