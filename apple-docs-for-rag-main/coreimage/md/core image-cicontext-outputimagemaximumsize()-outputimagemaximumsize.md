

- Core Image
- CIContext
-  outputImageMaximumSize() 

Instance Method

# outputImageMaximumSize()

Returns the maximum size allowed for any image created by the context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
func outputImageMaximumSize() -> CGSize
```

## Discussion

Some contexts limit the maximum size of an image that can be created by them. For example, the maximum size might reflect a limitation in the underlying graphics hardware.

## See Also

### Determining the Allowed Extents for Images Used by a Context

func inputImageMaximumSize() -> CGSize

Returns the maximum size allowed for any image rendered into the context.

