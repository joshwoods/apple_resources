

- Combine
- Just
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

