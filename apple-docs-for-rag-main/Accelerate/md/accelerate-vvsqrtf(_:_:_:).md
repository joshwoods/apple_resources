

- Accelerate
-  vvsqrtf(\_:\_:\_:) 

Function

# vvsqrtf(\_:\_:\_:)

Calculates the square root of each element in an array of single-precision values.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vvsqrtf(
    _: UnsafeMutablePointer,
    _: UnsafePointer,
    _: UnsafePointer
)
```

## Discussion

### Parameters:

parameter 1  
The output array, *y*.

parameter 2  
The input array, *x*.

parameter 3  
The number of elements in the arrays.

The following code shows an example of using vvsqrtf(_:_:_:).

- Swift
- Objective-C

```
var x: [Float] = [100, 10000, 64, 144]
var y = [Float](repeating: 0, count: x.count)
var n = Int32(x.count)

vvsqrtf(&y, &x, &n)

print(y) // [10.0, 100.0, 8.0, 12.0]
```

```
float x[] = {100, 10000, 64, 144};
float y[4];
int n = 4;

vvsqrtf(y, x, &n);

NSLog(@"y: [%lf, %lf, %lf, %lf]", y[0], y[1], y[2], y[3]);
```

## See Also

### Array-Oriented Arithmetic and Auxiliary Functions

static func ceil&lt;U>(U) -> [Double]

Returns the ceiling of each element in a vector of double-precision values.

static func ceil&lt;U>(U) -> [Float]

Returns the ceiling of each element in a vector of single-precision values.

static func ceil&lt;U, V>(U, result: inout V)

Calculates the ceiling of each element in a vector of double-precision values.

static func ceil&lt;U, V>(U, result: inout V)

Calculates the ceiling of each element in a vector of single-precision values.

static func copysign&lt;U, V>(magnitudes: U, signs: V) -> [Double]

Returns each single-precision element in the magnitudes vector, setting its sign to the corresponding elements in the signs vector.

static func copysign&lt;U, V>(magnitudes: U, signs: V) -> [Float]

Returns each single-precision element in the magnitudes vector, setting its sign to the corresponding elements in the signs vector.

static func copysign&lt;T, U, V>(magnitudes: T, signs: U, result: inout V)

Calculates each double-precision element in the magnitudes vector, setting its sign to the corresponding elements in the signs vector.

static func copysign&lt;T, U, V>(magnitudes: T, signs: U, result: inout V)

Calculates each single-precision element in the magnitudes vector, setting its sign to the corresponding elements in the signs vector.

static func floor&lt;U>(U) -> [Double]

Returns the floor of each element in a vector of double-precision values.

static func floor&lt;U>(U) -> [Float]

Returns the floor of each element in a vector of single-precision values.

static func floor&lt;U, V>(U, result: inout V)

Calculates the floor of each element in a vector of double-precision values.

static func floor&lt;U, V>(U, result: inout V)

Calculates the floor of each element in a vector of single-precision values.

static func nearestInteger&lt;U>(U) -> [Double]

Returns the nearest integer to each element in a vector of double-precision values.

static func nearestInteger&lt;U>(U) -> [Float]

Returns the nearest integer to each element in a vector of single-precision values.

static func nearestInteger&lt;U, V>(U, result: inout V)

Calculates the nearest integer to each element in a vector of double-precision values.

