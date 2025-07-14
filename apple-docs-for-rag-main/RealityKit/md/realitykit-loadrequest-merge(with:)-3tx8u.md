

- RealityKit
- LoadRequest
-  merge(with:) 

Instance Method

# merge(with:)

Combines elements from this publisher with those from another publisher of the same type, delivering an interleaved sequence of elements.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func merge(with other: Self) -> Publishers.MergeMany
```

## Parameters 

`other`  

Another publisher of this publisher’s type.

## Return Value

A publisher that emits an event when either upstream publisher emits an event.

