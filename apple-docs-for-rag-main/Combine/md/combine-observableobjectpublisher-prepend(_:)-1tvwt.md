

- Combine
- ObservableObjectPublisher
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

