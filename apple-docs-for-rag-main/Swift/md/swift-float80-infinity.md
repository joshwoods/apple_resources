

- Swift
- Float80
-  infinity 

Type Property

# infinity

Positive infinity.

macOS 10.10+

``` source
static var infinity: Float80 { get }
```

## Discussion

Infinity compares greater than all finite numbers and equal to other infinite values.

```
let x = Double.greatestFiniteMagnitude
let y = x * 2
// y == Double.infinity
// y > x
```

