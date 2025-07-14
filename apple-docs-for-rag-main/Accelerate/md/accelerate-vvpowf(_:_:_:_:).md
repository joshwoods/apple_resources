

- Accelerate
-  vvpowf(\_:\_:\_:\_:) 

Function

# vvpowf(\_:\_:\_:\_:)

Raises each element in an array to the power of the corresponding element in a second array of single-precision values.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vvpowf(
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
The exponent input array, *y*.

parameter 3  
The base input array, *x*.

parameter 4  
The number of elements in the arrays.

The following code shows an example of using vvpowf(_:_:_:_:):

- Swift
- Objective-C

```
var x: [Float] = [3, 2, 10, 6]
var y: [Float] = [2, 4, 3, 2]
var z = [Float](repeating: 0, count: x.count)
var n = Int32(x.count)

vvpowf(&z, &y, &x, &n)

print(z) // [9.0, 16.0, 1000.0, 36.0]
```

```
float x[] = {3, 2, 10, 6};
float y[] = {2, 4, 3, 2};
float z[4];
int n = 4;

vvpowf(z, y, x, &n);

NSLog(@"z: [%lf, %lf, %lf, %lf]", z[0], z[1], z[2], z[3]);
```

The following special values of `x` and `y` produce the given value of `z`:

| x (base)          | y (exponent) | z (result) |
|-------------------|--------------|------------|
| `odd integer, 0` | `+/-0`       | `+/-0`     |
| `otherwise, 0`   | `+/-0`       | `+0`       |
| `+/-inf`          | `-1`         | `1`        |
| `NaN`             | `+1`         | `1`        |
| `+/-0`            | `NaN`        | `1`        |
| `-inf`            | `|x|1`      | `+0`       |
| `+inf`            | `|x|1`      | `+inf`     |
| `odd integer, 0` | `-inf`       | `-inf`     |
| `otherwise, 0`   | `-inf`       | `+inf`     |
| `0`              | `+inf`       | `+inf`     |
| `non-integer`     | `

## See Also

### Array-Oriented Power Functions

static func pow&lt;U, V>(bases: U, exponents: V) -> [Double]

Returns each double-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

static func pow&lt;U, V>(bases: U, exponents: V) -> [Float]

Returns each single-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

static func pow&lt;T, U, V>(bases: T, exponents: U, result: inout V)

Calculates each double-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

static func pow&lt;T, U, V>(bases: T, exponents: U, result: inout V)

Calculates each single-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

func vvpow(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Raises each element in an array to the power of the corresponding element in a second array of double-precision values.

