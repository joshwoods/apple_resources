

- Swift
- Float80
-  zero 

Type Property

# zero

The zero value.

macOS 10.10+

``` source
static var zero: Self { get }
```

Available when `Self` conforms to `ExpressibleByIntegerLiteral`.

## Discussion

Zero is the identity element for addition. For any value, `x + .zero == x` and `.zero + x == x`.

