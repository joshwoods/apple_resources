

- Combine
-  Publishers 

Enumeration

# Publishers

A namespace for types that serve as publishers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Publishers
```

## Overview

The various operators defined as extensions on Publisher implement their functionality as classes or structures that extend this enumeration. For example, the `contains(_:)` operator returns a `Publishers.Contains` instance.

## Topics

### Convenience Publishers

struct Sequence

A publisher that publishes a given sequence of elements.

struct Catch

A publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher.

### Working with Subscribers

struct ReceiveOn

A publisher that delivers elements to its downstream subscriber on a specific scheduler.

struct SubscribeOn

A publisher that receives elements from an upstream publisher on a specific scheduler.

### Mapping Elements

struct Map

A publisher that transforms all elements from the upstream publisher with a provided closure.

struct TryMap

A publisher that transforms all elements from the upstream publisher with a provided error-throwing closure.

struct MapError

A publisher that converts any failure from the upstream publisher into a new error.

struct Scan

A publisher that transforms elements from the upstream publisher by providing the current element to a closure along with the last value returned by the closure.

struct TryScan

A publisher that transforms elements from the upstream publisher by providing the current element to a failable closure along with the last value returned by the closure.

struct SetFailureType

A publisher that appears to send a specified failure type.

### Filtering Elements

struct Filter

A publisher that republishes all elements that match a provided closure.

struct TryFilter

A publisher that republishes all elements that match a provided error-throwing closure.

struct CompactMap

A publisher that republishes all non-nil results of calling a closure with each received element.

struct TryCompactMap

A publisher that republishes all non-nil results of calling an error-throwing closure with each received element.

struct RemoveDuplicates

A publisher that publishes only elements that don’t match the previous element.

struct TryRemoveDuplicates

A publisher that publishes only elements that don’t match the previous element, as evaluated by a provided error-throwing closure.

struct ReplaceEmpty

A publisher that replaces an empty stream with a provided element.

struct ReplaceError

A publisher that replaces any errors in the stream with a provided element.

### Reducing Elements

struct Collect

A publisher that buffers items.

struct CollectByCount

A publisher that buffers a maximum number of items.

struct CollectByTime

A publisher that buffers and periodically publishes its items.

enum TimeGroupingStrategy

A strategy for collecting received elements.

struct IgnoreOutput

A publisher that ignores all upstream elements, but passes along the upstream publisher’s completion state (finished or failed).

struct Reduce

A publisher that applies a closure to all received elements and produces an accumulated value when the upstream publisher finishes.

struct TryReduce

A publisher that applies an error-throwing closure to all received elements and produces an accumulated value when the upstream publisher finishes.

### Applying Mathematical Operations on Elements

struct Count

A publisher that publishes the number of elements received from the upstream publisher.

struct Comparison

A publisher that republishes items from another publisher only if each new item is in increasing order from the previously-published item.

struct TryComparison

A publisher that republishes items from another publisher only if each new item is in increasing order from the previously-published item, and fails if the ordering logic throws an error.

### Applying Matching Criteria to Elements

struct Contains

A publisher that emits a Boolean value when it receives a specific element from its upstream publisher.

struct ContainsWhere

A publisher that emits a Boolean value upon receiving an element that satisfies the predicate closure.

struct TryContainsWhere

A publisher that emits a Boolean value upon receiving an element that satisfies the throwing predicate closure.

struct AllSatisfy

A publisher that publishes a single Boolean value that indicates whether all received elements pass a given predicate.

struct TryAllSatisfy

A publisher that publishes a single Boolean value that indicates whether all received elements pass a given error-throwing predicate.

### Applying Sequence Operations to Elements

struct DropUntilOutput

A publisher that ignores elements from the upstream publisher until it receives an element from second publisher.

struct Drop

A publisher that omits a specified number of elements before republishing later elements.

struct DropWhile

A publisher that omits elements from an upstream publisher until a given closure returns false.

struct TryDropWhile

A publisher that omits elements from an upstream publisher until a given error-throwing closure returns false.

struct Concatenate

A publisher that emits all of one publisher’s elements before those from another publisher.

struct PrefixWhile

A publisher that republishes elements while a predicate closure indicates publishing should continue.

struct TryPrefixWhile

A publisher that republishes elements while an error-throwing predicate closure indicates publishing should continue.

struct PrefixUntilOutput

A publisher that republishes elements until another publisher emits an element.

### Selecting Specific Elements

struct First

A publisher that publishes the first element of a stream, then finishes.

struct FirstWhere

A publisher that only publishes the first element of a stream to satisfy a predicate closure.

struct TryFirstWhere

A publisher that only publishes the first element of a stream to satisfy a throwing predicate closure.

struct Last

A publisher that waits until after the stream finishes, and then publishes the last element of the stream.

struct LastWhere

A publisher that waits until after the stream finishes and then publishes the last element of the stream that satisfies a predicate closure.

struct TryLastWhere

A publisher that waits until after the stream finishes and then publishes the last element of the stream that satisfies an error-throwing predicate closure.

struct Output

A publisher that publishes elements specified by a range in the sequence of published elements.

### Combining Elements from Multiple Publishers

struct CombineLatest

A publisher that receives and combines the latest elements from two publishers.

struct CombineLatest3

A publisher that receives and combines the latest elements from three publishers.

struct CombineLatest4

A publisher that receives and combines the latest elements from four publishers.

struct Merge

A publisher created by applying the merge function to two upstream publishers.

struct Merge3

A publisher created by applying the merge function to three upstream publishers.

struct Merge4

A publisher created by applying the merge function to four upstream publishers.

struct Merge5

A publisher created by applying the merge function to five upstream publishers.

struct Merge6

A publisher created by applying the merge function to six upstream publishers.

struct Merge7

A publisher created by applying the merge function to seven upstream publishers.

struct Merge8

A publisher created by applying the merge function to eight upstream publishers.

struct MergeMany

A publisher created by applying the merge function to an arbitrary number of upstream publishers.

struct Zip

A publisher created by applying the zip function to two upstream publishers.

struct Zip3

A publisher created by applying the zip function to three upstream publishers.

struct Zip4

A publisher created by applying the zip function to four upstream publishers.

### Republishing Elements by Subscribing to New Publishers

struct FlatMap

A publisher that transforms elements from an upstream publisher into a new publisher.

struct SwitchToLatest

A publisher that flattens nested publishers.

### Handling Errors

struct AssertNoFailure

A publisher that raises a fatal error upon receiving any failure, and otherwise republishes all received input.

struct Catch

A publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher.

struct TryCatch

A publisher that handles errors from an upstream publisher by replacing the failed publisher with another publisher or producing a new error.

struct Retry

A publisher that attempts to recreate its subscription to a failed upstream publisher.

### Controlling Timing

struct MeasureInterval

A publisher that measures and emits the time interval between events received from an upstream publisher.

struct Debounce

A publisher that publishes elements only after a specified time interval elapses between events.

struct Delay

A publisher that delays delivery of elements and completion to the downstream receiver.

struct Throttle

A publisher that publishes either the most-recent or first element published by the upstream publisher in a specified time interval.

struct Timeout

A publisher that terminates publishing if the upstream publisher exceeds a specified time interval without producing an element.

### Encoding and Decoding

struct Decode

A publisher that decodes elements received from an upstream publisher, using a given decoder.

struct Encode

A publisher that encodes elements received from an upstream publisher, using a given encoder.

### Identifying Properties with Key Paths

struct MapKeyPath

A publisher that publishes the value of a key path.

struct MapKeyPath2

A publisher that publishes the values of two key paths as a tuple.

struct MapKeyPath3

A publisher that publishes the values of three key paths as a tuple.

### Working with Multiple Subscribers

class Multicast

A publisher that uses a subject to deliver elements to multiple subscribers.

class Share

A publisher that shares the output of an upstream publisher with multiple subscribers.

### Buffering Elements

struct Buffer

A publisher that buffers elements from an upstream publisher.

enum BufferingStrategy

A strategy that handles exhaustion of a buffer’s capacity.

enum PrefetchStrategy

A strategy for filling a buffer.

### Using Explicit Publisher Connections

class Autoconnect

A publisher that automatically connects to an upstream connectable publisher.

struct MakeConnectable

A publisher that provides explicit connectability to another publisher.

### Debugging

struct Breakpoint

A publisher that raises a debugger signal when a provided closure needs to stop the process in the debugger.

struct HandleEvents

A publisher that performs the specified closures when publisher events occur.

struct Print

A publisher that prints log messages for all publishing events, optionally prefixed with a given string.

## See Also

### Publishers

protocol Publisher

Declares that a type can transmit a sequence of values over time.

struct AnyPublisher

A publisher that performs type erasure by wrapping another publisher.

struct Published

A type that publishes a property marked with an attribute.

protocol Cancellable

A protocol indicating that an activity or action supports cancellation.

class AnyCancellable

A type-erasing cancellable object that executes a provided closure when canceled.

