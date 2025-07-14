

- ML Compute
- MLCArithmeticOperation
-  MLCArithmeticOperation.multiplyNoNaN Deprecated

Case

# MLCArithmeticOperation.multiplyNoNaN

Calculates the element-wise product of the inputs, and returns `0` when the result isn’t a number or infinity.

iOS 14.5–17.4DeprecatediPadOS 14.5–17.4DeprecatedMac Catalyst 14.5–17.4DeprecatedmacOS 11.3–14.3DeprecatedtvOS 14.5–17.4Deprecated

``` source
case multiplyNoNaN
```

## Discussion

Returns `0` if `y` in `x * y` is zero, even if `x` isn’t a number (`NaN)` or infinity (`INF)`.

## See Also

### Basic Operations

case add

Calculates the element-wise sum of the inputs.

Deprecated

case subtract

Calculates the element-wise difference between the inputs.

Deprecated

case multiply

Calculates the element-wise product of the inputs.

Deprecated

case divide

Calculates the element-wise division of the inputs.

Deprecated

case divideNoNaN

Calculates the element-wise division of the inputs, and returns `0` if the denominator is `0`.

Deprecated

case min

Calculates the element-wise minimum of the inputs.

Deprecated

case max

Calculates the element-wise maximum the inputs.

Deprecated

