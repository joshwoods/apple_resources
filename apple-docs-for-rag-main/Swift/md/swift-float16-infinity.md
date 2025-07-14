

- Swift
- Float16
-  infinity 

Type Property

# infinity

Positive infinity.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var infinity: Float16 { get }
```

## Discussion

Infinity compares greater than all finite numbers and equal to other infinite values.

```
let x = Double.greatestFiniteMagnitude
let y = x * 2
// y == Double.infinity
// y > x
```

