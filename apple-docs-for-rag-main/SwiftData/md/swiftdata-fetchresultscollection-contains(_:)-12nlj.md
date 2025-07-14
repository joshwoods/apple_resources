

- SwiftData
- FetchResultsCollection
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the sequence contains the given element.

SwiftDataSwiftiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

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

