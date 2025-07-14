

- Create ML Components
- SlidingWindows
-  trimmingPrefix(\_:) 

Instance Method

# trimmingPrefix(\_:)

Returns a new collection of the same type by removing `prefix` from the start of the collection.

Create ML ComponentsSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func trimmingPrefix(_ prefix: Prefix) -> Self.SubSequence where Prefix : Sequence, Self.Element == Prefix.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`prefix`  

The collection to remove from this collection.

## Return Value

A collection containing the elements of the collection that are not removed by `prefix`.

