

- Create ML Components
- SlidingWindows
-  index(\_:offsetBy:) 

Instance Method

# index(\_:offsetBy:)

Returns an index that is the specified distance from the given index.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func index(
    _ i: Int,
    offsetBy distance: Int
) -> Int
```

## Parameters 

`i`  

A valid index of the collection.

`distance`  

The distance to offset `i`.

## Return Value

An index offset by `distance` from the index `i`.

## Discussion

The value passed as `distance` must not offset `i` beyond the bounds of the collection.

