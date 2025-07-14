

- Core ML
- MLSequence
-  init(empty:) 

Initializer

# init(empty:)

Creates an empty sequence of strings or integers.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
convenience init(empty type: MLFeatureType)
```

## Parameters 

`type`  

An MLFeatureType instance that determines the sequence’s element type, which must be either MLFeatureType.string or MLFeatureType.int64.

## See Also

### Creating a Sequence

convenience init(strings: [String])

Creates a sequence of strings from a string array.

convenience init(int64s: [NSNumber])

Creates a sequence of integers from an array of numbers.

