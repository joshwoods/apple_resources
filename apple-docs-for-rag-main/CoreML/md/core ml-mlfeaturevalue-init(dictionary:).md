

- Core ML
- MLFeatureValue
-  init(dictionary:) 

Initializer

# init(dictionary:)

Creates a feature value that contains a dictionary of numbers.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
convenience init(dictionary value: [AnyHashable : NSNumber]) throws
```

## Parameters 

`value`  

A dictionary of numbers.

## See Also

### Creating Collection Feature Values

convenience init(sequence: MLSequence)

Creates a feature value that contains a sequence.

