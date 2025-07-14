

- Foundation
- SortDescriptor
-  init(\_:comparing:) 

Initializer

# init(\_:comparing:)

Creates a sort descriptor using a sort descriptor and a type that you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init?(
    _ descriptor: NSSortDescriptor,
    comparing comparedType: Compared.Type
) where Compared : NSObject
```

## Parameters 

`descriptor`  

A sort descriptor.

`comparedType`  

The type that the sort descriptor compares.

## Discussion

Returns `nil` if there isn’t a SortDescriptor equivalent to the NSSortDescriptor you specify, or if the selector to NSSortDescriptor isn’t one of the standard string comparison algorithms or `compare(_:)`.

The comparison for the created SortDescriptor uses the selector to the associated NSSortDescriptor directly, so in cases where the comparison of NSSortDescriptor might crash, the SortDescriptor comparison crashes as well.

