

- Swift
- Float80
-  ulpOfOne 

Type Property

# ulpOfOne

The unit in the last place of 1.0.

macOS 10.10+

``` source
static var ulpOfOne: Float80 { get }
```

## Discussion

The positive difference between 1.0 and the next greater representable number. The `ulpOfOne` constant corresponds to the C macros `FLT_EPSILON`, `DBL_EPSILON`, and others with a similar purpose.

