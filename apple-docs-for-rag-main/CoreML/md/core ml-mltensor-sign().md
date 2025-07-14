

- Core ML
- MLTensor
-  sign() 

Instance Method

# sign()

Returns the sign of the tensor’s elements.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func sign() -> MLTensor
```

## Discussion

This operation returns `1.0` if the correspnding element is greater than `0`, `-1.0` if it is less than `0`, `-0.0` if it is equal to `-0.0`, and `+0.0` if it is equal to `+0.0`.

