

- Combine
- Publishers
- Publishers.SwitchToLatest
-  Publisher Implementations 

API Collection

# Publisher Implementations

## Topics

### Instance Properties

var values: AsyncThrowingPublisher&lt;Self>

The elements produced by the publisher, as a throwing asynchronous sequence.

var values: AsyncPublisher&lt;Self>

The elements produced by the publisher, as an asynchronous sequence.

### Instance Methods

func allSatisfy((Self.Output) -> Bool) -> Publishers.AllSatisfy&lt;Self>

Publishes a single Boolean value that indicates whether all received elements pass a given predicate.

func append(Self.Output...) -> Publishers.Concatenate&lt;Self, Publishers.Sequence&lt;[Self.Output], Self.Failure>>

Appends a publisher’s output with the specified elements.

func assertNoFailure(String, file: StaticString, line: UInt) -> Publishers.AssertNoFailure&lt;Self>

Raises a fatal error when its upstream publisher fails, and otherwise republishes all received input.

func assign(to: inout Published&lt;Self.Output>.Publisher)

Republishes elements received from a publisher, by assigning them to a property marked as a publisher.

func assign&lt;Root>(to: ReferenceWritableKeyPath&lt;Root, Self.Output>, on: Root) -> AnyCancellable

Assigns each element from a publisher to a property on an object.

func breakpoint(receiveSubscription: ((any Subscription) -> Bool)?, receiveOutput: ((Self.Output) -> Bool)?, receiveCompletion: ((Subscribers.Completion&lt;Self.Failure>) -> Bool)?) -> Publishers.Breakpoint&lt;Self>

Raises a debugger signal when a provided closure needs to stop the process in the debugger.

func breakpointOnError() -> Publishers.Breakpoint&lt;Self>

Raises a debugger signal upon receiving a failure.

func buffer(size: Int, prefetch: Publishers.PrefetchStrategy, whenFull: Publishers.BufferingStrategy&lt;Self.Failure>) -> Publishers.Buffer&lt;Self>

Buffers elements received from an upstream publisher.

func `catch`&lt;P>((Self.Failure) -> P) -> Publishers.Catch&lt;Self, P>

Handles errors from an upstream publisher by replacing it with another publisher.

func collect() -> Publishers.Collect&lt;Self>

Collects all received elements, and emits a single array of the collection when the upstream publisher finishes.

func collect(Int) -> Publishers.CollectByCount&lt;Self>

Collects up to the specified number of elements, and then emits a single array of the collection.

func collect&lt;S>(Publishers.TimeGroupingStrategy&lt;S>, options: S.SchedulerOptions?) -> Publishers.CollectByTime&lt;Self, S>

Collects elements by a given time-grouping strategy, and emits a single array of the collection.

func combineLatest&lt;P>(P) -> Publishers.CombineLatest&lt;Self, P>

Subscribes to an additional publisher and publishes a tuple upon receiving output from either publisher.

func combineLatest&lt;P, T>(P, (Self.Output, P.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest&lt;Self, P>, T>

Subscribes to an additional publisher and invokes a closure upon receiving output from either publisher.

func combineLatest&lt;P, Q>(P, Q) -> Publishers.CombineLatest3&lt;Self, P, Q>

Subscribes to two additional publishers and publishes a tuple upon receiving output from any of the publishers.

func combineLatest&lt;P, Q, T>(P, Q, (Self.Output, P.Output, Q.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest3&lt;Self, P, Q>, T>

Subscribes to two additional publishers and invokes a closure upon receiving output from any of the publishers.

func combineLatest&lt;P, Q, R>(P, Q, R) -> Publishers.CombineLatest4&lt;Self, P, Q, R>

Subscribes to three additional publishers and publishes a tuple upon receiving output from any of the publishers.

func combineLatest&lt;P, Q, R, T>(P, Q, R, (Self.Output, P.Output, Q.Output, R.Output) -> T) -> Publishers.Map&lt;Publishers.CombineLatest4&lt;Self, P, Q, R>, T>

Subscribes to three additional publishers and invokes a closure upon receiving output from any of the publishers.

func compactMap&lt;T>((Self.Output) -> T?) -> Publishers.CompactMap&lt;Self, T>

Calls a closure with each received element and publishes any returned optional that has a value.

func contains(Self.Output) -> Publishers.Contains&lt;Self>

Publishes a Boolean value upon receiving an element equal to the argument.

func contains(where: (Self.Output) -> Bool) -> Publishers.ContainsWhere&lt;Self>

Publishes a Boolean value upon receiving an element that satisfies the predicate closure.

func count() -> Publishers.Count&lt;Self>

Publishes the number of elements received from the upstream publisher.

func debounce&lt;S>(for: S.SchedulerTimeType.Stride, scheduler: S, options: S.SchedulerOptions?) -> Publishers.Debounce&lt;Self, S>

Publishes elements only after a specified time interval elapses between events.

func decode&lt;Item, Coder>(type: Item.Type, decoder: Coder) -> Publishers.Decode&lt;Self, Item, Coder>

Decodes the output from the upstream using a specified decoder.

func delay&lt;S>(for: S.SchedulerTimeType.Stride, tolerance: S.SchedulerTimeType.Stride?, scheduler: S, options: S.SchedulerOptions?) -> Publishers.Delay&lt;Self, S>

Delays delivery of all output to the downstream receiver by a specified amount of time on a particular scheduler.

func drop&lt;P>(untilOutputFrom: P) -> Publishers.DropUntilOutput&lt;Self, P>

Ignores elements from the upstream publisher until it receives an element from a second publisher.

func drop(while: (Self.Output) -> Bool) -> Publishers.DropWhile&lt;Self>

Omits elements from the upstream publisher until a given closure returns false, before republishing all remaining elements.

func dropFirst(Int) -> Publishers.Drop&lt;Self>

Omits the specified number of elements before republishing subsequent elements.

func encode&lt;Coder>(encoder: Coder) -> Publishers.Encode&lt;Self, Coder>

Encodes the output from upstream using a specified encoder.

func eraseToAnyPublisher() -> AnyPublisher&lt;Self.Output, Self.Failure>

Wraps this publisher with a type eraser.

func filter((Self.Output) -> Bool) -> Publishers.Filter&lt;Self>

Republishes all elements that match a provided closure.

func first() -> Publishers.First&lt;Self>

Publishes the first element of a stream, then finishes.

func first(where: (Self.Output) -> Bool) -> Publishers.FirstWhere&lt;Self>

Publishes the first element of a stream to satisfy a predicate closure, then finishes normally.

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;Publishers.SetFailureType&lt;P, Self.Failure>, Self>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;P, Self>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func flatMap&lt;T, P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;P, Self>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func flatMap&lt;P>(maxPublishers: Subscribers.Demand, (Self.Output) -> P) -> Publishers.FlatMap&lt;P, Publishers.SetFailureType&lt;Self, P.Failure>>

Transforms all elements from an upstream publisher into a new publisher up to a maximum number of publishers you specify.

func handleEvents(receiveSubscription: ((any Subscription) -> Void)?, receiveOutput: ((Self.Output) -> Void)?, receiveCompletion: ((Subscribers.Completion&lt;Self.Failure>) -> Void)?, receiveCancel: (() -> Void)?, receiveRequest: ((Subscribers.Demand) -> Void)?) -> Publishers.HandleEvents&lt;Self>

Performs the specified closures when publisher events occur.

func ignoreOutput() -> Publishers.IgnoreOutput&lt;Self>

Ignores all upstream elements, but passes along the upstream publisher’s completion state (finished or failed).

func last() -> Publishers.Last&lt;Self>

Publishes the last element of a stream, after the stream finishes.

func last(where: (Self.Output) -> Bool) -> Publishers.LastWhere&lt;Self>

Publishes the last element of a stream that satisfies a predicate closure, after upstream finishes.

func makeConnectable() -> Publishers.MakeConnectable&lt;Self>

Creates a connectable wrapper around the publisher.

func map&lt;T>((Self.Output) -> T) -> Publishers.Map&lt;Self, T>

Transforms all elements from the upstream publisher with a provided closure.

func map&lt;T>(KeyPath&lt;Self.Output, T>) -> Publishers.MapKeyPath&lt;Self, T>

Publishes the value of a key path.

func map&lt;T0, T1>(KeyPath&lt;Self.Output, T0>, KeyPath&lt;Self.Output, T1>) -> Publishers.MapKeyPath2&lt;Self, T0, T1>

Publishes the values of two key paths as a tuple.

func map&lt;T0, T1, T2>(KeyPath&lt;Self.Output, T0>, KeyPath&lt;Self.Output, T1>, KeyPath&lt;Self.Output, T2>) -> Publishers.MapKeyPath3&lt;Self, T0, T1, T2>

Publishes the values of three key paths as a tuple.

func mapError&lt;E>((Self.Failure) -> E) -> Publishers.MapError&lt;Self, E>

Converts any failure from the upstream publisher into a new error.

func max() -> Publishers.Comparison&lt;Self>

Publishes the maximum value received from the upstream publisher, after it finishes.

func max(by: (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided ordering closure.

func measureInterval&lt;S>(using: S, options: S.SchedulerOptions?) -> Publishers.MeasureInterval&lt;Self, S>

Measures and emits the time interval between events received from an upstream publisher.

func merge(with: Self) -> Publishers.MergeMany&lt;Self>

Combines elements from this publisher with those from another publisher of the same type, delivering an interleaved sequence of elements.

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

func min() -> Publishers.Comparison&lt;Self>

Publishes the minimum value received from the upstream publisher, after it finishes.

func min(by: (Self.Output, Self.Output) -> Bool) -> Publishers.Comparison&lt;Self>

Publishes the minimum value received from the upstream publisher, after it finishes.

func multicast&lt;S>(() -> S) -> Publishers.Multicast&lt;Self, S>

Applies a closure to create a subject that delivers elements to subscribers.

func multicast&lt;S>(subject: S) -> Publishers.Multicast&lt;Self, S>

Provides a subject to deliver elements to multiple subscribers.

func output(at: Int) -> Publishers.Output&lt;Self>

Publishes a specific element, indicated by its index in the sequence of published elements.

func output&lt;R>(in: R) -> Publishers.Output&lt;Self>

Publishes elements specified by their range in the sequence of published elements.

func prefix(Int) -> Publishers.Output&lt;Self>

Republishes elements up to the specified maximum count.

func prefix&lt;P>(untilOutputFrom: P) -> Publishers.PrefixUntilOutput&lt;Self, P>

Republishes elements until another publisher emits an element.

func prefix(while: (Self.Output) -> Bool) -> Publishers.PrefixWhile&lt;Self>

Republishes elements while a predicate closure indicates publishing should continue.

func prepend(Self.Output...) -> Publishers.Concatenate&lt;Publishers.Sequence&lt;[Self.Output], Self.Failure>, Self>

Prefixes a publisher’s output with the specified values.

func print(String, to: (any TextOutputStream)?) -> Publishers.Print&lt;Self>

Prints log messages for all publishing events.

func receive&lt;S>(on: S, options: S.SchedulerOptions?) -> Publishers.ReceiveOn&lt;Self, S>

Specifies the scheduler on which to receive elements from the publisher.

func reduce&lt;T>(T, (T, Self.Output) -> T) -> Publishers.Reduce&lt;Self, T>

Applies a closure that collects each element of a stream and publishes a final result upon completion.

func removeDuplicates() -> Publishers.RemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element.

func removeDuplicates(by: (Self.Output, Self.Output) -> Bool) -> Publishers.RemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element, as evaluated by a provided closure.

func replaceEmpty(with: Self.Output) -> Publishers.ReplaceEmpty&lt;Self>

Replaces an empty stream with the provided element.

func replaceError(with: Self.Output) -> Publishers.ReplaceError&lt;Self>

Replaces any errors in the stream with the provided element.

func replaceNil&lt;T>(with: T) -> Publishers.Map&lt;Self, T>

Replaces nil elements in the stream with the provided element.

func retry(Int) -> Publishers.Retry&lt;Self>

Attempts to recreate a failed subscription with the upstream publisher up to the number of times you specify.

func scan&lt;T>(T, (T, Self.Output) -> T) -> Publishers.Scan&lt;Self, T>

Transforms elements from the upstream publisher by providing the current element to a closure along with the last value returned by the closure.

func setFailureType&lt;E>(to: E.Type) -> Publishers.SetFailureType&lt;Self, E>

Changes the failure type declared by the upstream publisher.

func share() -> Publishers.Share&lt;Self>

Shares the output of an upstream publisher with multiple subscribers.

func sink(receiveCompletion: (Subscribers.Completion&lt;Self.Failure>) -> Void, receiveValue: (Self.Output) -> Void) -> AnyCancellable

Attaches a subscriber with closure-based behavior.

func sink(receiveValue: (Self.Output) -> Void) -> AnyCancellable

Attaches a subscriber with closure-based behavior to a publisher that never fails.

func subscribe&lt;S>(S)

Attaches the specified subscriber to this publisher.

func subscribe&lt;S>(S) -> AnyCancellable

Attaches the specified subject to this publisher.

func subscribe&lt;S>(on: S, options: S.SchedulerOptions?) -> Publishers.SubscribeOn&lt;Self, S>

Specifies the scheduler on which to perform subscribe, cancel, and request operations.

func switchToLatest() -> Publishers.SwitchToLatest&lt;Self.Output, Publishers.SetFailureType&lt;Self, Self.Output.Failure>>

Republishes elements sent by the most recently received publisher.

func throttle&lt;S>(for: S.SchedulerTimeType.Stride, scheduler: S, latest: Bool) -> Publishers.Throttle&lt;Self, S>

Publishes either the most-recent or first element published by the upstream publisher in the specified time interval.

func timeout&lt;S>(S.SchedulerTimeType.Stride, scheduler: S, options: S.SchedulerOptions?, customError: (() -> Self.Failure)?) -> Publishers.Timeout&lt;Self, S>

Terminates publishing if the upstream publisher exceeds the specified time interval without producing an element.

func tryAllSatisfy((Self.Output) throws -> Bool) -> Publishers.TryAllSatisfy&lt;Self>

Publishes a single Boolean value that indicates whether all received elements pass a given error-throwing predicate.

func tryCatch&lt;P>((Self.Failure) throws -> P) -> Publishers.TryCatch&lt;Self, P>

Handles errors from an upstream publisher by either replacing it with another publisher or throwing a new error.

func tryCompactMap&lt;T>((Self.Output) throws -> T?) -> Publishers.TryCompactMap&lt;Self, T>

Calls an error-throwing closure with each received element and publishes any returned optional that has a value.

func tryContains(where: (Self.Output) throws -> Bool) -> Publishers.TryContainsWhere&lt;Self>

Publishes a Boolean value upon receiving an element that satisfies the throwing predicate closure.

func tryDrop(while: (Self.Output) throws -> Bool) -> Publishers.TryDropWhile&lt;Self>

Omits elements from the upstream publisher until an error-throwing closure returns false, before republishing all remaining elements.

func tryFilter((Self.Output) throws -> Bool) -> Publishers.TryFilter&lt;Self>

Republishes all elements that match a provided error-throwing closure.

func tryFirst(where: (Self.Output) throws -> Bool) -> Publishers.TryFirstWhere&lt;Self>

Publishes the first element of a stream to satisfy a throwing predicate closure, then finishes normally.

func tryLast(where: (Self.Output) throws -> Bool) -> Publishers.TryLastWhere&lt;Self>

Publishes the last element of a stream that satisfies an error-throwing predicate closure, after the stream finishes.

func tryMap&lt;T>((Self.Output) throws -> T) -> Publishers.TryMap&lt;Self, T>

Transforms all elements from the upstream publisher with a provided error-throwing closure.

func tryMax(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the maximum value received from the upstream publisher, using the provided error-throwing closure to order the items.

func tryMin(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryComparison&lt;Self>

Publishes the minimum value received from the upstream publisher, using the provided error-throwing closure to order the items.

func tryPrefix(while: (Self.Output) throws -> Bool) -> Publishers.TryPrefixWhile&lt;Self>

Republishes elements while an error-throwing predicate closure indicates publishing should continue.

func tryReduce&lt;T>(T, (T, Self.Output) throws -> T) -> Publishers.TryReduce&lt;Self, T>

Applies an error-throwing closure that collects each element of a stream and publishes a final result upon completion.

func tryRemoveDuplicates(by: (Self.Output, Self.Output) throws -> Bool) -> Publishers.TryRemoveDuplicates&lt;Self>

Publishes only elements that don’t match the previous element, as evaluated by a provided error-throwing closure.

func tryScan&lt;T>(T, (T, Self.Output) throws -> T) -> Publishers.TryScan&lt;Self, T>

Transforms elements from the upstream publisher by providing the current element to an error-throwing closure along with the last value returned by the closure.

func zip&lt;P>(P) -> Publishers.Zip&lt;Self, P>

Combines elements from another publisher and deliver pairs of elements as tuples.

func zip&lt;P, T>(P, (Self.Output, P.Output) -> T) -> Publishers.Map&lt;Publishers.Zip&lt;Self, P>, T>

Combines elements from another publisher and delivers a transformed output.

func zip&lt;P, Q>(P, Q) -> Publishers.Zip3&lt;Self, P, Q>

Combines elements from two other publishers and delivers groups of elements as tuples.

func zip&lt;P, Q, R>(P, Q, R) -> Publishers.Zip4&lt;Self, P, Q, R>

Combines elements from three other publishers and delivers groups of elements as tuples.

func zip&lt;P, Q, T>(P, Q, (Self.Output, P.Output, Q.Output) -> T) -> Publishers.Map&lt;Publishers.Zip3&lt;Self, P, Q>, T>

Combines elements from two other publishers and delivers a transformed output.

func zip&lt;P, Q, R, T>(P, Q, R, (Self.Output, P.Output, Q.Output, R.Output) -> T) -> Publishers.Map&lt;Publishers.Zip4&lt;Self, P, Q, R>, T>

Combines elements from three other publishers and delivers a transformed output.

