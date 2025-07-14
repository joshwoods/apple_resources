

- Swift
- Float80
-  isCanonical 

Instance Property

# isCanonical

A Boolean value indicating whether the instance’s representation is in its canonical form.

macOS 10.10+

``` source
var isCanonical: Bool { get }
```

## Discussion

The IEEE 754 specification defines a *canonical*, or preferred, encoding of a floating-point value. On platforms that fully support IEEE 754, every `Float` or `Double` value is canonical, but non-canonical values can exist on other platforms or for other types. Some examples:

- On platforms that flush subnormal numbers to zero (such as armv7 with the default floating-point environment), Swift interprets subnormal `Float` and `Double` values as non-canonical zeros. (In Swift 5.1 and earlier, `isCanonical` is `true` for these values, which is the incorrect value.)

- On i386 and x86_64, `Float80` has a number of non-canonical encodings. “Pseudo-NaNs”, “pseudo-infinities”, and “unnormals” are interpreted as non-canonical NaN encodings. “Pseudo-denormals” are interpreted as non-canonical encodings of subnormal values.

- Decimal floating-point types admit a large number of non-canonical encodings. Consult the IEEE 754 standard for additional details.

