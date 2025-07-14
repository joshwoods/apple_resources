

- Combine
- Publisher
-  prepend(\_:) 

Instance Method

# prepend(\_:)

Prefixes the output of this publisher with the elements emitted by the given publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func prepend(_ publisher: P) -> Publishers.Concatenate where P : Publisher, Self.Failure == P.Failure, Self.Output == P.Output
```

## Parameters 

`publisher`  

The prefixing publisher.

## Return Value

A publisher that prefixes the prefixing publisher’s elements prior to this publisher’s elements.

## Discussion

Use prepend(_:) to publish values from two publishers when you need to prepend one publisher’s elements to another.

In the example below, a publisher of `prefixValues` publishes its elements before the `dataElements` publishes its elements:

```
let prefixValues = [0, 1, 255]
let dataElements = (0...10)
cancellable = dataElements.publisher
    .prepend(prefixValues.publisher)
    .sink { print("\($0)", terminator: " ") }

// Prints: "0 1 255 0 1 2 3 4 5 6 7 8 9 10"
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

func append&lt;S>(S) -> Publishers.Concatenate&lt;Self, Publishers.Sequence&lt;S, Self.Failure>>

Appends a publisher’s output with the specified sequence.

func append&lt;P>(P) -> Publishers.Concatenate&lt;Self, P>

Appends the output of this publisher with the elements emitted by the given publisher.

func prepend(Self.Output...) -> Publishers.Concatenate&lt;Publishers.Sequence&lt;[Self.Output], Self.Failure>, Self>

Prefixes a publisher’s output with the specified values.

func prepend&lt;S>(S) -> Publishers.Concatenate&lt;Publishers.Sequence&lt;S, Self.Failure>, Self>

Prefixes a publisher’s output with the specified sequence.

func prefix(Int) -> Publishers.Output&lt;Self>

Republishes elements up to the specified maximum count.

func prefix(while: (Self.Output) -> Bool) -> Publishers.PrefixWhile&lt;Self>

Republishes elements while a predicate closure indicates publishing should continue.

func tryPrefix(while: (Self.Output) throws -> Bool) -> Publishers.TryPrefixWhile&lt;Self>

Republishes elements while an error-throwing predicate closure indicates publishing should continue.

func prefix&lt;P>(untilOutputFrom: P) -> Publishers.PrefixUntilOutput&lt;Self, P>

Republishes elements until another publisher emits an element.

