

- Swift
- FloatingPoint
-  infinity 

Type Property

# infinity

Positive infinity.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var infinity: Self { get }
```

**Required**

## Discussion

Infinity compares greater than all finite numbers and equal to other infinite values.

```
let x = Double.greatestFiniteMagnitude
let y = x * 2
// y == Double.infinity
// y > x
```

