

- Combine
- Publishers
- Publishers.Merge7
-  prepend(\_:) 

Instance Method

# prepend(\_:)

Prefixes a publisher’s output with the specified values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func prepend(_ elements: Self.Output...) -> Publishers.Concatenate, Self>
```

## Parameters 

`elements`  

The elements to publish before this publisher’s elements.

## Return Value

A publisher that prefixes the specified elements prior to this publisher’s elements.

## Discussion

Use prepend(_:) when you need to prepend specific elements before the output of a publisher.

In the example below, the prepend(_:) operator publishes the provided elements before republishing all elements from `dataElements`:

```
let dataElements = (0...10)
cancellable = dataElements.publisher
    .prepend(0, 1, 255)
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

func prefix(Int) -> Publishers.Output&lt;Self>

Republishes elements up to the specified maximum count.

func prefix(while: (Self.Output) -> Bool) -> Publishers.PrefixWhile&lt;Self>

Republishes elements while a predicate closure indicates publishing should continue.

func tryPrefix(while: (Self.Output) throws -> Bool) -> Publishers.TryPrefixWhile&lt;Self>

Republishes elements while an error-throwing predicate closure indicates publishing should continue.

func prefix&lt;P>(untilOutputFrom: P) -> Publishers.PrefixUntilOutput&lt;Self, P>

Republishes elements until another publisher emits an element.

