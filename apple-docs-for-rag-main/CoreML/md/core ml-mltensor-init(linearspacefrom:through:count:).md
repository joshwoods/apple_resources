

- Core ML
- MLTensor
-  init(linearSpaceFrom:through:count:) 

Initializer

# init(linearSpaceFrom:through:count:)

Creates a one-dimensional tensor representing a sequence from a starting value, up to and including an end value, spaced evenly to generate the number of values specified.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    linearSpaceFrom start: Float,
    through end: Float,
    count: Int
)
```

## Parameters 

`start`  

The starting value to use for the sequence. If the sequence contains any values, the first one is `start`.

`end`  

An end value to limit the sequence. `end` is the last element of the resulting sequence.

`count`  

The number of values in the resulting sequence. `count` must be positive and greater than `1`.

