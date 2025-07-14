

- Accelerate
-  vvremainderf(\_:\_:\_:\_:) 

Function

# vvremainderf(\_:\_:\_:\_:)

Calculates the remainder after dividing each element in an array by the corresponding element in a second array of single-precision values.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vvremainderf(
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

- termparameter 4: The number of elements in the arrays.

The following code shows an example of using vvremainderf(_:_:_:_:):

- Swift
- Objective-C

```
var x: [Float] = [7, 4, 3, 4]
var y: [Float] = [2, 5, 10, 30]
var z = [Float](repeating: 0, count: x.count)
var n = Int32(x.count)

vvremainderf(&z, &y, &x, &n)

print(z) // [2.0, 1.0, 1.0, -2.0]
```

```
float x[] = {7, 4, 3, 4};
float y[] = {2, 5, 10, 30};
float z[4];
int n = 4;

vvremainderf(z, y, x, &n);

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

