

- Combine
- Empty
-  prefix(untilOutputFrom:) 

Instance Method

# prefix(untilOutputFrom:)

Republishes elements until another publisher emits an element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func prefix(untilOutputFrom publisher: P) -> Publishers.PrefixUntilOutput where P : Publisher
```

## Parameters 

`publisher`  

A second publisher.

## Return Value

A publisher that republishes elements until the second publisher publishes an element.

## Discussion

After the second publisher publishes an element, the publisher returned by this method finishes.

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

func prefix(Int) -> Publishers.Output&lt;Self>

Republishes elements up to the specified maximum count.

func prefix(while: (Self.Output) -> Bool) -> Publishers.PrefixWhile&lt;Self>

Republishes elements while a predicate closure indicates publishing should continue.

func tryPrefix(while: (Self.Output) throws -> Bool) -> Publishers.TryPrefixWhile&lt;Self>

Republishes elements while an error-throwing predicate closure indicates publishing should continue.

