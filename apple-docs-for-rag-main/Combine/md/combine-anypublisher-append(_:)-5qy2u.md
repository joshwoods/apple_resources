

- Combine
- AnyPublisher
-  append(\_:) 

Instance Method

# append(\_:)

Appends a publisher’s output with the specified elements.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func append(_ elements: Self.Output...) -> Publishers.Concatenate>
```

## Parameters 

`elements`  

Elements to publish after this publisher’s elements.

## Return Value

A publisher that appends the specifiecd elements after this publisher’s elements.

## Discussion

Use append(_:) when you need to prepend specific elements after the output of a publisher.

In the example below, the append(_:) operator publishes the provided elements after republishing all elements from `dataElements`:

```
let dataElements = (0...10)
cancellable = dataElements.publisher
    .append(0, 1, 255)
    .sink { print("\($0)", terminator: " ") }

// Prints: "0 1 2 3 4 5 6 7 8 9 10 0 1 255"
```

