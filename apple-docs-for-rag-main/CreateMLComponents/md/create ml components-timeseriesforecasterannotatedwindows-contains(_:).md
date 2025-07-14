

- Create ML Components
- TimeSeriesForecasterAnnotatedWindows
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the sequence contains the given element.

Create ML ComponentsSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func contains(_ element: Self.Element) -> Bool
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`element`  

The element to find in the sequence.

## Return Value

`true` if the element was found in the sequence; otherwise, `false`.

## Discussion

This example checks to see whether a favorite actor is in an array storing a movie’s cast.

```
let cast = ["Vivien", "Marlon", "Kim", "Karl"]
print(cast.contains("Marlon"))
// Prints "true"
print(cast.contains("James"))
// Prints "false"
```

Complexity

O(*n*), where *n* is the length of the sequence.

