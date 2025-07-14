

- Accelerate
-  BNNSArithmeticSelect 

Global Variable

# BNNSArithmeticSelect

An operation that selects elements from either its second or third input based on the corresponding value of its first input.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var BNNSArithmeticSelect: BNNSArithmeticFunction { get }
```

## Discussion

This function returns values using the following operation:

```
 out = in1 ? in2 : in3
```

## See Also

### Ternary Arithmetic Functions

var BNNSArithmeticMultiplyAdd: BNNSArithmeticFunction

An operation that calculates the element-wise fused multiply-add of its three inputs.

