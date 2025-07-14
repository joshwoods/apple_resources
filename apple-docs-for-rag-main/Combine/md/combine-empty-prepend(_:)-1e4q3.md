

- Combine
- Empty
-  prepend(\_:) 

Instance Method

# prepend(\_:)

Prefixes a publisher’s output with the specified sequence.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func prepend(_ elements: S) -> Publishers.Concatenate, Self> where S : Sequence, Self.Output == S.Element
```

## Parameters 

`elements`  

A sequence of elements to publish before this publisher’s elements.

## Return Value

A publisher that prefixes the sequence of elements prior to this publisher’s elements.

## Discussion

Use prepend(_:) to publish values from two publishers when you need to prepend one publisher’s elements to another.

In this example the prepend(_:) operator publishes the provided sequence before republishing all elements from `dataElements`:

```
let prefixValues = [0, 1, 255]
let dataElements = (0...10)
cancellable = dataElements.publisher
    .prepend(prefixValues)
    .sink { print("\($0)", terminator: " ") }

// Prints: "0 1 255 0 1 2 3 4 5 6 7 8 9 10"
```

