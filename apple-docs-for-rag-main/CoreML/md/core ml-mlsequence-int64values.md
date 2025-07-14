

- Core ML
- MLSequence
-  int64Values 

Instance Property

# int64Values

An array of 64-bit integers in the sequence.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
var int64Values: [NSNumber] { get }
```

## Discussion

Only use this property when the sequence’s type is MLFeatureType.int64.

## See Also

### Retrieving the Sequence’s Values

var stringValues: [String]

An array of strings in the sequence.

