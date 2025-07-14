

- SwiftData
- FetchResultsCollection
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value indicating whether the collection contains the given sequence.

SwiftDataSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func contains(_ other: C) -> Bool where C : Collection, Self.Element == C.Element
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`other`  

A sequence to search for within this collection.

## Return Value

`true` if the collection contains the specified sequence, otherwise `false`.

