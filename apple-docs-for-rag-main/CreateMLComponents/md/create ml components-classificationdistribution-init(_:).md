

- Create ML Components
- ClassificationDistribution
-  init(\_:) 

Initializer

# init(\_:)

Creates a classification distribution.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(_ classifications: C) where C : Collection, C.Element == Classification
```

## Parameters 

`classifications`  

A collection of classifications.

## Discussion

Precondition

The classifications must contain unique labels.

