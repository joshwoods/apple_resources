

- XPC
- XPCArray
-  map(\_:) 

Instance Method

# map(\_:)

Returns an array containing the results of mapping the given closure over the sequence’s elements.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+watchOS 9.0+

``` source
func map(_ transform: (XPCArray.IndexValuePair) throws -> ReturnType) rethrows -> [ReturnType]
```

## Parameters 

`transform`  

A mapping closure. `transform` accepts an element of this sequence as its parameter and returns a transformed value of the same or of a different type.

