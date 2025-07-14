

- Combine
- Just
-  Publisher Operators 

API Collection

# Publisher Operators

Methods that create downstream publishers or subscribers to act on the elements they receive.

## Overview

Use operators to assemble a chain of republishers, optionally ending with a subscriber, that processes elements produced by upstream publishers. Each operator creates and configures an instance of a Publisher or Subscriber, and subscribes it to the publisher that you call the method on.

In the following example, a sequence publisher emits the integers 1, 2, 3, 4, and 5. A filter(_:) operator creates a Publishers.Filter publisher to only republish even values. A second operator creates a Subscribers.Sink subscriber to print out each value received. The sink subscriber automatically subscribes to the filter publisher, at which point the filter publisher subscribes to its upstream publisher, the sequence publisher.

```
let cancellable = [1, 2, 3, 4, 5].publisher
    .filter {
        $0 % 2 == 0
    }
    .sink {
        print ("Even number: \($0)")
    }
// Prints:
// Even number: 2
// Even number: 4
```

## Topics

### Working with Subscribers

func receive&lt;S>(subscriber: S)

Attaches the specified subscriber to this publisher.

func subscribe&lt;S>(S)

Attaches the specified subscriber to this publisher.

func subscribe&lt;S>(S) -> AnyCancellable

Attaches the specified subject to this publisher.

### Mapping Elements

func map&lt;T>((Output) -> T) -> Just&lt;T>

func tryMap&lt;T>((Output) throws -> T) -> Result&lt;T, any Error>.Publisher

func mapError&lt;E>((Just&lt;Output>.Failure) -> E) -> Result&lt;Output, E>.Publisher

func replaceNil&lt;T>(with: T) -> Publishers.Map&lt;Self, T>

Replaces nil elements in the stream with the provided element.

func scan&lt;T>(T, (T, Output) -> T) -> Result&lt;T, Just&lt;Output>.Failure>.Publisher

func tryScan&lt;T>(T, (T, Output) throws -> T) -> Result&lt;T, any Error>.Publisher

func setFailureType&lt;E>(to: E.Type) -> Result&lt;Output, E>.Publisher

### Filtering Elements

func filter((Output) -> Bool) -> Optional&lt;Output>.Publisher

func tryFilter((Self.Output) throws -> Bool) -> Publishers.TryFilter&lt;Self>

Republishes all elements that match a provided error-throwing closure.

func compactMap&lt;T>((Output) -> T?) -> Optional&lt;T>.Publisher

func tryCompactMap&lt;T>((Self.Output) throws -> T?) -> Publishers.TryCompactMap&lt;Self, T>

Calls an error-throwing closure with each received element and publishes any returned optional that has a value.

func removeDuplicates() -> Just&lt;Output>

func removeDuplicates(by: (Output, Output) -> Bool) -> Just&lt;Output>

func tryRemoveDuplicates(by: (Output, Output) throws -> Bool) -> Result&lt;Output, any Error>.Publisher

func replaceEmpty(with: Output) -> Just&lt;Output>

func replaceError(with: Output) -> Just&lt;Output>

### Reducing Elements

func collect() -> Just&lt;[Output]>

func collect(Int) -> Publishers.CollectByCount&lt;Self>

Collects up to the specified number of elements, and then emits a single array of the collection.

func collect&lt;S>(Publishers.TimeGroupingStrategy&lt;S>, options: S.SchedulerOptions?) -> Publishers.CollectByTime&lt;Self, S>

Collects elements by a given time-grouping strategy, and emits a single array of the collection.

func ignoreOutput() -> Empty&lt;Output, Just&lt;Output>.Failure>

func reduce&lt;T>(T, (T, Output) -> T) -> Result&lt;T, Just&lt;Output>.Failure>.Publisher

func tryReduce&lt;T>(T, (T, Output) throws -> T) -> Result&lt;T, any Error>.Publisher

### Applying Mathematical Operations on Elements

func count() -> Just&lt;Int>

func max() -> Just&lt;Output>

func max(by: (Output, Output) -> Bool) -> Just&lt;Output>

func tryMax(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided error-throwing closure to order the items.

func min() -> Just&lt;Output>

func min(by: (Output, Output) -> Bool) -> Just&lt;Output>

func tryMin(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the minimum value received from the upstream publisher, using the provided error-throwing closure to order the items.

### Applying Matching Criteria to Elements

func contains(Output) -> Just&lt;Bool>

func contains(where: (Output) -> Bool) -> Just&lt;Bool>

func tryContains(where: (Output) throws -> Bool) -> Result&lt;Bool, any Error>.Publisher

func allSatisfy((Output) -> Bool) -> Just&lt;Bool>

func tryAllSatisfy((Output) throws -> Bool) -> Result&lt;Bool, any Error>.Publisher

### Applying Sequence Operations to Elements

func drop&lt;P>(untilOutputFrom: P) -> Publishers.DropUntilOutput&lt;Self, P>

Ignores elements from the upstream publisher until it receives an element from a second publisher.

func dropFirst(Int) -> Optional&lt;Output>.Publisher

func drop(while: (Output) -> Bool) -> Optional&lt;Output>.Publisher

func tryDrop(while: (Self.Output) throws -> Bool) -> Publishers.TryDropWhile&lt;Self>

Omits elements from the upstream publisher until an error-throwing closure returns false, before republishing all remaining elements.

func append(Output...) -> Publishers.Sequence&lt;[Output], Just&lt;Output>.Failure>

func append&lt;S>(S) -> Publishers.Sequence&lt;[Output], Just&lt;Output>.Failure>

func prepend&lt;S>(S) -> Publishers.Sequence&lt;[Output], Just&lt;Output>.Failure>

func prepend(Output...) -> Publishers.Sequence&lt;[Output], Just&lt;Output>.Failure>

func prefix(Int) -> Optional&lt;Output>.Publisher

func prefix(while: (Output) -> Bool) -> Optional&lt;Output>.Publisher

func tryPrefix(while: (Self.Output) throws -> Bool) -> Publishers.TryPrefixWhile&lt;Self>

Republishes elements while an error-throwing predicate closure indicates publishing should continue.

func prefix&lt;P>(untilOutputFrom: P) -> Publishers.PrefixUntilOutput&lt;Self, P>

Republishes elements until another publisher emits an element.

### Selecting Specific Elements

func first() -> Just&lt;Output>

func first(where: (Output) -> Bool) -> Optional&lt;Output>.Publisher

func tryFirst(where: (Self.Output) throws -> Bool) -> Publishers.TryFirstWhere&lt;Self>

Publishes the first element of a stream to satisfy a throwing predicate closure, then finishes normally.

func last() -> Just&lt;Output>

func last(where: (Output) -> Bool) -> Optional&lt;Output>.Publisher

func tryLast(where: (Self.Output) throws -> Bool) -> Publishers.TryLastWhere&lt;Self>

Publishes the last element of a stream that satisfies an error-throwing predicate closure, after the stream finishes.

func output(at: Int) -> Optional&lt;Output>.Publisher

func output&lt;R>(in: R) -> Optional&lt;Output>.Publisher

### Collecting and Republishing the Latest Elements from Multiple Publishers

func combineLatest&lt;P, T>(P, (Self.Output, P.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest&lt;Self, P>, T>

Subscribes to an additional publisher and invokes a closure upon receiving output from either publisher.

func combineLatest&lt;P>(P) -> Publishers.CombineLatest&lt;Self, P>

Subscribes to an additional publisher and publishes a tuple upon receiving output from either publisher.

func combineLatest&lt;P, Q, T>(P, Q, (Self.Output, P.Output, Q.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest3&lt;Self, P, Q>, T>

Subscribes to two additional publishers and invokes a closure upon receiving output from any of the publishers.

func combineLatest&lt;P, Q>(P, Q) -> Publishers.CombineLatest3&lt;Self, P, Q>

Subscribes to two additional publishers and publishes a tuple upon receiving output from any of the publishers.

func combineLatest&lt;P, Q, R, T>(P, Q, R, (Self.Output, P.Output, Q.Output, R.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest4&lt;Self, P, Q, R>, T>

Subscribes to three additional publishers and invokes a closure upon receiving output from any of the publishers.

func combineLatest&lt;P, Q, R>(P, Q, R) -> Publishers.CombineLatest4&lt;Self, P, Q, R>

Subscribes to three additional publishers and publishes a tuple upon receiving output from any of the publishers.

### Republishing Elements from Multiple Publishers as an Interleaved Stream

func merge&lt;B, C>(with: B, C) -> Publishers.Merge3&lt;Self, B, C>

Combines elements from this publisher with those from two other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D>(with: B, C, D) -> Publishers.Merge4&lt;Self, B, C, D>

Combines elements from this publisher with those from three other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D, E>(with: B, C, D, E) -> Publishers.Merge5&lt;Self, B, C, D, E>

Combines elements from this publisher with those from four other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D, E, F>(with: B, C, D, E, F) -> Publishers.Merge6&lt;Self, B, C, D, E, F>

Combines elements from this publisher with those from five other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D, E, F, G>(with: B, C, D, E, F, G) -> Publishers.Merge7&lt;Self, B, C, D, E, F, G>

Combines elements from this publisher with those from six other publishers, delivering an interleaved sequence of elements.

func merge&lt;B, C, D, E, F, G, H>(with: B, C, D, E, F, G, H) -> Publishers.Merge8&lt;Self, B, C, D, E, F, G, H>

Combines elements from this publisher with those from seven other publishers, delivering an interleaved sequence of elements.

### Collecting and Republishing the Oldest Unconsumed Elements from Multiple Publishers

func zip&lt;P>(P) -> Publishers.Zip&lt;Self, P>

Combines elements from another publisher and deliver pairs of elements as tuples.

func zip&lt;P, T>(P, (Self.Output, P.Output) -> T) -> Publishers.Map&lt;Publishers.Zip&lt;Self, P>, T>

Combines elements from another publisher and delivers a transformed output.

func zip&lt;P, Q>(P, Q) -> Publishers.Zip3&lt;Self, P, Q>

Combines elements from two other publishers and delivers groups of elements as tuples.

func zip&lt;P, Q, T>(P, Q, (Self.Output, P.Output, Q.Output) -> T) -> Publishers.Map&lt;Publishers.Zip3&lt;Self, P, Q>, T>

Combines elements from two other publishers and delivers a transformed output.

func zip&lt;P, Q, R>(P, Q, R) -> Publishers.Zip4&lt;Self, P, Q, R>

Combines elements from three other publishers and delivers groups of elements as tuples.

func zip&lt;P, Q, R, T>(P, Q, R, (Self.Output, P.Output, Q.Output, R.Output) -> T) -> Publishers.Map&lt;Publishers.Zip4&lt;Self, P, Q, R>, T>

Combines elements from three other publishers and delivers a transformed output.

### Republishing Elements by Subscribing to New Publishers

func flatMap&lt;T, P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;P, Self>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;P, Publishers.SetFailureType&lt;Self, P.Failure>>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;P, Self>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;Publishers.SetFailureType&lt;P, Self.Failure>, Self>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func switchToLatest() -> Publishers.SwitchToLatest&lt;Self.Output, Publishers.SetFailureType&lt;Self, Self.Output.Failure>>

Republishes elements sent by the most recently received publisher.

### Handling Errors

func assertNoFailure(String, file: StaticString, line: UInt) -> Publishers.AssertNoFailure&lt;Self>

Raises a fatal error when its upstream publisher fails, and otherwise republishes all received input.

func `catch`&lt;P>((Self.Failure) -> P) -> Publishers.Catch&lt;Self, P>

Handles errors from an upstream publisher by replacing it with another publisher.

func tryCatch&lt;P>((Self.Failure) throws -> P) -> Publishers.TryCatch&lt;Self, P>

Handles errors from an upstream publisher by either replacing it with another publisher or throwing a new error.

func retry(Int) -> Just&lt;Output>

### Controlling Timing

func measureInterval&lt;S>(using: S, options: S.SchedulerOptions?) -> Publishers.MeasureInterval&lt;Self, S>

Measures and emits the time interval between events received from an upstream publisher.

func debounce&lt;S>(for: S.SchedulerTimeType.Stride, scheduler: S, options: S.SchedulerOptions?) -> Publishers.Debounce&lt;Self, S>

Publishes elements only after a specified time interval elapses between events.

func delay&lt;S>(for: S.SchedulerTimeType.Stride, tolerance: S.SchedulerTimeType.Stride?, scheduler: S, options: S.SchedulerOptions?) -> Publishers.Delay&lt;Self, S>

Delays delivery of all output to the downstream receiver by a specified amount of time on a particular scheduler.

func throttle&lt;S>(for: S.SchedulerTimeType.Stride, scheduler: S, latest: Bool) -> Publishers.Throttle&lt;Self, S>

Publishes either the most-recent or first element published by the upstream publisher in the specified time interval.

func timeout&lt;S>(S.SchedulerTimeType.Stride, scheduler: S, options: S.SchedulerOptions?, customError: (() -> Self.Failure)?) -> Publishers.Timeout&lt;Self, S>

Terminates publishing if the upstream publisher exceeds the specified time interval without producing an element.

### Encoding and Decoding

func decode&lt;Item, Coder>(type: Item.Type, decoder: Coder) -> Publishers.Decode&lt;Self, Item, Coder>

Decodes the output from the upstream using a specified decoder.

func encode&lt;Coder>(encoder: Coder) -> Publishers.Encode&lt;Self, Coder>

Encodes the output from upstream using a specified encoder.

### Identifying Properties with Key Paths

func map&lt;T>(KeyPath&lt;Self.Output, T>) -> Publishers.MapKeyPath&lt;Self, T>

Publishes the value of a key path.

func map&lt;T0, T1>(KeyPath&lt;Self.Output, T0>, KeyPath&lt;Self.Output, T1>) -> Publishers.MapKeyPath2&lt;Self, T0, T1>

Publishes the values of two key paths as a tuple.

func map&lt;T0, T1, T2>(KeyPath&lt;Self.Output, T0>, KeyPath&lt;Self.Output, T1>, KeyPath&lt;Self.Output, T2>) -> Publishers.MapKeyPath3&lt;Self, T0, T1, T2>

Publishes the values of three key paths as a tuple.

### Working with Multiple Subscribers

func multicast&lt;S>(() -> S) -> Publishers.Multicast&lt;Self, S>

Applies a closure to create a subject that delivers elements to subscribers.

func multicast&lt;S>(subject: S) -> Publishers.Multicast&lt;Self, S>

Provides a subject to deliver elements to multiple subscribers.

func share() -> Publishers.Share&lt;Self>

Shares the output of an upstream publisher with multiple subscribers.

### Buffering Elements

func buffer(size: Int, prefetch: Publishers.PrefetchStrategy, whenFull: Publishers.BufferingStrategy&lt;Self.Failure>) -> Publishers.Buffer&lt;Self>

Buffers elements received from an upstream publisher.

### Performing Type-Erasure

func eraseToAnyPublisher() -> AnyPublisher&lt;Self.Output, Self.Failure>

Wraps this publisher with a type eraser.

### Specifying Schedulers

func subscribe&lt;S>(on: S, options: S.SchedulerOptions?) -> Publishers.SubscribeOn&lt;Self, S>

Specifies the scheduler on which to perform subscribe, cancel, and request operations.

func receive&lt;S>(on: S, options: S.SchedulerOptions?) -> Publishers.ReceiveOn&lt;Self, S>

Specifies the scheduler on which to receive elements from the publisher.

### Adding Explicit Connectability

func makeConnectable() -> Publishers.MakeConnectable&lt;Self>

Creates a connectable wrapper around the publisher.

### Connecting Simple Subscribers

func assign&lt;Root>(to: ReferenceWritableKeyPath&lt;Root, Self.Output>, on: Root) -> AnyCancellable

Assigns each element from a publisher to a property on an object.

func assign(to: inout Published&lt;Self.Output>.Publisher)

Republishes elements received from a publisher, by assigning them to a property marked as a publisher.

func sink(receiveCompletion: (Subscribers.Completion&lt;Self.Failure>) -> Void, receiveValue: (Self.Output) -> Void) -> AnyCancellable

Attaches a subscriber with closure-based behavior.

func sink(receiveValue: (Self.Output) -> Void) -> AnyCancellable

Attaches a subscriber with closure-based behavior to a publisher that never fails.

### Debugging

func breakpoint(receiveSubscription: ((any Subscription) -> Bool)?, receiveOutput: ((Self.Output) -> Bool)?, receiveCompletion: ((Subscribers.Completion&lt;Self.Failure>) -> Bool)?) -> Publishers.Breakpoint&lt;Self>

Raises a debugger signal when a provided closure needs to stop the process in the debugger.

func breakpointOnError() -> Publishers.Breakpoint&lt;Self>

Raises a debugger signal upon receiving a failure.

func handleEvents(receiveSubscription: ((any Subscription) -> Void)?, receiveOutput: ((Self.Output) -> Void)?, receiveCompletion: ((Subscribers.Completion&lt;Self.Failure>) -> Void)?, receiveCancel: (() -> Void)?, receiveRequest: ((Subscribers.Demand) -> Void)?) -> Publishers.HandleEvents&lt;Self>

Performs the specified closures when publisher events occur.

func print(String, to: (any TextOutputStream)?) -> Publishers.Print&lt;Self>

Prints log messages for all publishing events.

