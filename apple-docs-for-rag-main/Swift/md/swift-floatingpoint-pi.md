

- Swift
- FloatingPoint
-  pi 

Type Property

# pi

The mathematical constant pi (π), approximately equal to 3.14159.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var pi: Self { get }
```

**Required**

## Discussion

When measuring an angle in radians, π is equivalent to a half-turn.

This value is rounded toward zero to keep user computations with angles from inadvertently ending up in the wrong quadrant. A type that conforms to the `FloatingPoint` protocol provides the value for `pi` at its best possible precision.

```
print(Double.pi)
// Prints "3.14159265358979"
```

