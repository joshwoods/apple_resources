

- Create ML
- MLHandActionClassifier
- MLHandActionClassifier.VideoAugmentationOptions
-  init(\_:) 

Initializer

# init(\_:)

Creates a new set from a finite sequence of items.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

``` source
init(_ sequence: S) where S : Sequence, Self.Element == S.Element
```

## Parameters 

`sequence`  

The elements to use as members of the new set.

## Discussion

Use this initializer to create a new set from an existing sequence, like an array or a range:

```
let validIndices = Set(0..

