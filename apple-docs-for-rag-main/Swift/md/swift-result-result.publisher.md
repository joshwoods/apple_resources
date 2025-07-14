

- Swift
- Result
-  Result.Publisher 

Structure

# Result.Publisher

The type of a Combine publisher that publishes this instance’s result to each subscriber exactly once, or fails immediately if the result indicates failure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Publisher
```

Available when `Failure` conforms to `Error`.

## Overview

If the result is `Swift/Result/success`, then the publisher waits until it receives a request for at least one value, then sends the output to all subscribers and finishes normally. If the result is `/Swift/Result/failure`, then the publisher sends the failure immediately upon subscription. This latter behavior is a contrast with Just, which always publishes a single value.

## Topics

### Declaring Publisher Topology

typealias Output

The kind of values published by this publisher.

### Creating a Result Publisher

init(Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>)

Creates a publisher that delivers the specified result.

init(Failure)

Creates a publisher that immediately terminates upon subscription with the given failure.

init(Result&lt;Success, Failure>.Publisher.Output)

Creates a publisher that sends the specified output to all subscribers and finishes normally.

### Inspecting Publisher Properties

let result: Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>

The result to deliver to each subscriber.

### Working with Subscribers

func receive&lt;S>(subscriber: S)

Attaches the specified subscriber to this publisher.

### Instance Methods

func allSatisfy((Result&lt;Success, Failure>.Publisher.Output) -> Bool) -> Result&lt;Bool, Failure>.Publisher

func collect() -> Result&lt;[Result&lt;Success, Failure>.Publisher.Output], Failure>.Publisher

func contains(Result&lt;Success, Failure>.Publisher.Output) -> Result&lt;Bool, Failure>.Publisher

func contains(where: (Result&lt;Success, Failure>.Publisher.Output) -> Bool) -> Result&lt;Bool, Failure>.Publisher

func count() -> Result&lt;Int, Failure>.Publisher

func first() -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>.Publisher

func ignoreOutput() -> Empty&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>

func last() -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>.Publisher

func map&lt;T>((Result&lt;Success, Failure>.Publisher.Output) -> T) -> Result&lt;T, Failure>.Publisher

func mapError&lt;E>((Failure) -> E) -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, E>.Publisher

func max() -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>.Publisher

func max(by: (Result&lt;Success, Failure>.Publisher.Output, Result&lt;Success, Failure>.Publisher.Output) -> Bool) -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>.Publisher

func min() -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>.Publisher

func min(by: (Result&lt;Success, Failure>.Publisher.Output, Result&lt;Success, Failure>.Publisher.Output) -> Bool) -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>.Publisher

func reduce&lt;T>(T, (T, Result&lt;Success, Failure>.Publisher.Output) -> T) -> Result&lt;T, Failure>.Publisher

func removeDuplicates() -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>.Publisher

func removeDuplicates(by: (Result&lt;Success, Failure>.Publisher.Output, Result&lt;Success, Failure>.Publisher.Output) -> Bool) -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>.Publisher

func replaceEmpty(with: Result&lt;Success, Failure>.Publisher.Output) -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>.Publisher

func replaceError(with: Result&lt;Success, Failure>.Publisher.Output) -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, Never>.Publisher

func retry(Int) -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, Failure>.Publisher

func scan&lt;T>(T, (T, Result&lt;Success, Failure>.Publisher.Output) -> T) -> Result&lt;T, Failure>.Publisher

func setFailureType&lt;E>(to: E.Type) -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, E>.Publisher

func tryAllSatisfy((Result&lt;Success, Failure>.Publisher.Output) throws -> Bool) -> Result&lt;Bool, any Error>.Publisher

func tryContains(where: (Result&lt;Success, Failure>.Publisher.Output) throws -> Bool) -> Result&lt;Bool, any Error>.Publisher

func tryMap&lt;T>((Result&lt;Success, Failure>.Publisher.Output) throws -> T) -> Result&lt;T, any Error>.Publisher

func tryMax(by: (Result&lt;Success, Failure>.Publisher.Output, Result&lt;Success, Failure>.Publisher.Output) throws -> Bool) -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, any Error>.Publisher

func tryMin(by: (Result&lt;Success, Failure>.Publisher.Output, Result&lt;Success, Failure>.Publisher.Output) throws -> Bool) -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, any Error>.Publisher

func tryReduce&lt;T>(T, (T, Result&lt;Success, Failure>.Publisher.Output) throws -> T) -> Result&lt;T, any Error>.Publisher

func tryRemoveDuplicates(by: (Result&lt;Success, Failure>.Publisher.Output, Result&lt;Success, Failure>.Publisher.Output) throws -> Bool) -> Result&lt;Result&lt;Success, Failure>.Publisher.Output, any Error>.Publisher

func tryScan&lt;T>(T, (T, Result&lt;Success, Failure>.Publisher.Output) throws -> T) -> Result&lt;T, any Error>.Publisher

### Default Implementations

Equatable Implementations

Publisher Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Success` conforms to `Equatable`, `Failure` conforms to `Equatable`, and `Failure` conforms to `Error`.

- Equatable

  Conforms when `Success` conforms to `Equatable`, `Failure` conforms to `Equatable`, and `Failure` conforms to `Error`.

- Publisher

## See Also

### Publishing a Result

var publisher: Result&lt;Success, Failure>.Publisher

A Combine publisher that publishes this instance’s result to each subscriber exactly once, or fails immediately if the result indicates failure.

