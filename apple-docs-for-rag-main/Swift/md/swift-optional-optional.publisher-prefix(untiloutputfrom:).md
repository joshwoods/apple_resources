

- Swift
- Optional
- Optional.Publisher
-  prefix(untilOutputFrom:) 

Instance Method

# prefix(untilOutputFrom:)

Republishes elements until another publisher emits an element.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

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

