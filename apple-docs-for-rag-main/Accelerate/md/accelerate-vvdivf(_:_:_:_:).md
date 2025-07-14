

- Accelerate
-  vvdivf(\_:\_:\_:\_:) 

Function

# vvdivf(\_:\_:\_:\_:)

Divides each element in an array by the corresponding value in a second array of single-precision values.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vvdivf(
    _: UnsafeMutablePointer,
    _: UnsafePointer,
    _: UnsafePointer,
    _: UnsafePointer
)
```

## Discussion

### Parameters:

parameter 1  
The output array, *z*.

parameter 2  
The numerators input array, *y*.

parameter 3  
The denominators input array, *x*.

parameter 4  
The number of elements in the arrays.

The following code shows an example of using vvdivf(_:_:_:_:):

- Swift
- Objective-C

```
var x: [Float] = [1, 2, 2, 4]
var y: [Float] = [1, 1, 10, 30]
var z = [Float](repeating: 0, count: x.count)
var n = Int32(x.count) 

vvdivf(&z, &y, &x, &n) 

print(z) // [1.0, 0.5, 5.0, 7.5]
```

```
float x[] = {1, 2, 2, 4};
float y[] = {1, 1, 10, 30};
float z[4];
int n = 4;

vvdivf(z, y, x, &n);

NSLog(@"z: [%lf, %lf, %lf, %lf]", z[0], z[1], z[2], z[3]);

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

