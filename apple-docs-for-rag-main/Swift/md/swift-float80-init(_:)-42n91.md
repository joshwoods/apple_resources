

- Swift
- Float80
-  init(\_:) 

Initializer

# init(\_:)

Creates a new value, rounded to the closest possible representation.

macOS 10.10+

``` source
init(_ v: Int)
```

## Discussion

If two representable values are equally close, the result is the value with more trailing zeros in its significand bit pattern.

