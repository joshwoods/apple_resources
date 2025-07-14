

- Accelerate
-  vvnintf(\_:\_:\_:) 

Function

# vvnintf(\_:\_:\_:)

Calculates the nearest integer for each element in an array of single-precision values.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vvnintf(
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

The following code shows an example of using vvnintf(_:_:_:).

- Swift
- Objective-C

```
var x: [Float] = [1.2, 5.5, 3.9, 26.9]
var y = [Float](repeating: 0, count: x.count)
var n = Int32(x.count)

vvnintf(&y, &x, &n)

print(y) // [1.0, 6.0, 4.0, 27.0]
```

```
float x[] = {1.2, 5.5, 3.9, 26.9};
float y[4];
int n = 4;

vvnintf(y, x, &n);

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

