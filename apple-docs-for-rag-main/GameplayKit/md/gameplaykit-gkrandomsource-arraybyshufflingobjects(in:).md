

- GameplayKit
- GKRandomSource
-  arrayByShufflingObjects(in:) 

Instance Method

# arrayByShufflingObjects(in:)

Returns an array whose contents are the same as those of the specified array, but in a random order determined by the random source.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func arrayByShufflingObjects(in array: [Any]) -> [Any]
```

## Parameters 

`array`  

An array of objects.

## Return Value

An array whose contents have been randomly shuffled.

## Discussion

Use this method with an instance of GKRandomSource (or of one of its subclasses) to randomly rearrange the contents of an array. For example, in a card game you might use this method to randomize an array of card objects.

