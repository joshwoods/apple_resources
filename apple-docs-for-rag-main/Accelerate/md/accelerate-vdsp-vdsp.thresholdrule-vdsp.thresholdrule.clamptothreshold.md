

- Accelerate
- vDSP
- vDSP.ThresholdRule
-  vDSP.ThresholdRule.clampToThreshold 

Case

# vDSP.ThresholdRule.clampToThreshold

Returns the threshold if the input value is less than threshold; otherwise returns the input value.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
case clampToThreshold
```

## Discussion

Use vDSP.ThresholdRule.clampToThreshold to calculate a new vector where the threshold operation sets all source values below the threshold to the threshold.

```
let source: [Float] = [12, 13, 14, 15, 16, 17, 18]

let destination = vDSP.threshold(source,
                                 to: 15,
                                 with: .clampToThreshold)

// Prints "[15.0, 15.0, 15.0, 15.0, 16.0, 17.0, 18.0]".
print(destination)
```

## See Also

### Threshold rules

case signedConstant(T)

Returns the negated constant if the input value is less than the threshold; otherwise returns the constant.

case zeroFill

Returns `0` if the input value is less than the threshold; otherwise returns the input value.

