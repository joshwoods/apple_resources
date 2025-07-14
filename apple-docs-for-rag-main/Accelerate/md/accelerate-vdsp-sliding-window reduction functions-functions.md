

- Accelerate
- vDSP
-  Sliding-window reduction functions 

API Collection

# Sliding-window reduction functions

Calculate maximum values and sums of values in a sliding window.

## Topics

### Sliding-window maximum functions

The functions in this group find the maximum value in a sliding window within an input vector.

vDSP_vswmax

Finds the maximum value in a sliding window at each possible position in a single-precision input vector.

vDSP_vswmaxD

Finds the maximum value in a sliding window at each possible position in a double-precision input vector.

### Sliding-window summation functions

The functions in this group calculate a sliding-window sum for a vector.

static func slidingWindowSum&lt;U>(U, usingWindowLength: Int) -> [Double]

Returns the double-precision sliding window sum of a vector.

static func slidingWindowSum&lt;U>(U, usingWindowLength: Int) -> [Float]

Returns the single-precision sliding window sum of a vector.

static func slidingWindowSum&lt;U, V>(U, usingWindowLength: Int, result: inout V)

Calculates the double-precision sliding window sum of a vector.

static func slidingWindowSum&lt;U, V>(U, usingWindowLength: Int, result: inout V)

Calculates the single-precision sliding window sum of a vector.

vDSP_vswsum

Finds the sum of values in a sliding window at each possible position in a single-precision input vector.

vDSP_vswsumD

Finds the sum of values in a sliding window at each possible position in a double-precision input vector.

