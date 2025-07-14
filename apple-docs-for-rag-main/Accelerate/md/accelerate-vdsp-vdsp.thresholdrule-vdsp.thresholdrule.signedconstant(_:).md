

- Accelerate
- vDSP
- vDSP.ThresholdRule
-  vDSP.ThresholdRule.signedConstant(\_:) 

Case

# vDSP.ThresholdRule.signedConstant(\_:)

Returns the negated constant if the input value is less than the threshold; otherwise returns the constant.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
case signedConstant(T)
```

## Discussion

Use vDSP.ThresholdRule.signedConstant(_:) to calculate a new vector where the threshold operation sets all source values below the threshold to the negated constant.

```
let source: [Float] = [12, 13, 14, 15, 16, 17, 18]

let destination = vDSP.threshold(source,
                                 to: 15,
                                 with: .signedConstant(99))

// Prints "[-99.0, -99.0, -99.0, 99.0, 99.0, 99.0, 99.0]".
print(destination)
```

## See Also

### Threshold rules

case clampToThreshold

Returns the threshold if the input value is less than threshold; otherwise returns the input value.

case zeroFill

Returns `0` if the input value is less than the threshold; otherwise returns the input value.

