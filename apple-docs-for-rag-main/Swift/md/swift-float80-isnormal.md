

- Swift
- Float80
-  isNormal 

Instance Property

# isNormal

A Boolean value indicating whether this instance is normal.

macOS 10.10+

``` source
var isNormal: Bool { get }
```

## Discussion

A *normal* value is a finite number that uses the full precision available to values of a type. Zero is neither a normal nor a subnormal number.

