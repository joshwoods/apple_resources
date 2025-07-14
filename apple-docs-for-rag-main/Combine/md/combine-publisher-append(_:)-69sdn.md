

- Combine
- Publisher
-  append(\_:) 

Instance Method

# append(\_:)

Appends a publisher’s output with the specified sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func append(_ elements: S) -> Publishers.Concatenate> where S : Sequence, Self.Output == S.Element
```

## Parameters 

`elements`  

A sequence of elements to publish after this publisher’s elements.

## Return Value

A publisher that appends the sequence of elements after this publisher’s elements.

## Discussion

Use append(_:) to append a sequence to the end of a publisher’s output.

In the example below, the append(_:) publisher republishes all elements from `groundTransport` until it finishes, then publishes the members of `airTransport`:

```
let groundTransport = ["car", "bus", "truck", "subway", "bicycle"]
let airTransport = ["parasail", "jet", "helicopter", "rocket"]
cancellable = groundTransport.publisher
    .append(airTransport)
    .sink { print("\($0)", terminator: " ") }

// Prints: "car bus truck subway bicycle parasail jet helicopter rocket"
```

## See Also

### Applying Sequence Operations to Elements

func drop&lt;P>(untilOutputFrom: P) -> Publishers.DropUntilOutput&lt;Self, P>

Ignores elements from the upstream publisher until it receives an element from a second publisher.

func dropFirst(Int) -> Publishers.Drop&lt;Self>

Omits the specified number of elements before republishing subsequent elements.

func drop(while: (Self.Output) -> Bool) -> Publishers.DropWhile&lt;Self>

Omits elements from the upstream publisher until a given closure returns false, before republishing all remaining elements.

func tryDrop(while: (Self.Output) throws -> Bool) -> Publishers.TryDropWhile&lt;Self>

Omits elements from the upstream publisher until an error-throwing closure returns false, before republishing all remaining elements.

func append(Self.Output...) -> Publishers.Concatenate&lt;Self, Publishers.Sequence&lt;[Self.Output], Self.Failure>>

Appends a publisher’s output with the specified elements.

func append&lt;P>(P) -> Publishers.Concatenate&lt;Self, P>

Appends the output of this publisher with the elements emitted by the given publisher.

func prepend(Self.Output...) -> Publishers.Concatenate&lt;Publishers.Sequence&lt;[Self.Output], Self.Failure>, Self>

Prefixes a publisher’s output with the specified values.

func prepend&lt;S>(S) -> Publishers.Concatenate&lt;Publishers.Sequence&lt;S, Self.Failure>, Self>

Prefixes a publisher’s output with the specified sequence.

func prepend&lt;P>(P) -> Publishers.Concatenate&lt;P, Self>

Prefixes the output of this publisher with the elements emitted by the given publisher.

func prefix(Int) -> Publishers.Output&lt;Self>

Republishes elements up to the specified maximum count.

func prefix(while: (Self.Output) -> Bool) -> Publishers.PrefixWhile&lt;Self>

Republishes elements while a predicate closure indicates publishing should continue.

func tryPrefix(while: (Self.Output) throws -> Bool) -> Publishers.TryPrefixWhile&lt;Self>

Republishes elements while an error-throwing predicate closure indicates publishing should continue.

func prefix&lt;P>(untilOutputFrom: P) -> Publishers.PrefixUntilOutput&lt;Self, P>

Republishes elements until another publisher emits an element.

