

- Core Image
- CIFilter
-  apply(\_:arguments:options:) 

Instance Method

# apply(\_:arguments:options:)

Produces a CIImage object by applying arguments to a kernel function and using options to control how the kernel function is evaluated.

macOS 10.4+

``` source
func apply(
    _ k: CIKernel,
    arguments args: [Any]?,
    options dict: [String : Any]? = nil
) -> CIImage?
```

## Parameters 

`k`  

A `CIKernel` object that contains a kernel function.

`args`  

The arguments that are type compatible with the function signature of the kernel function.

`dict`  

A dictionary that contains options (key-value pairs) to control how the kernel function is evaluated.

## Return Value

The CIImage object produced by a filter.

## Discussion

If you are implementing a custom filter, this method needs to be called from within the outputImage method in order to apply your kernel function to the CIImage object. You can pass any of the keys defined in Options for Applying a Filter, along with appropriate values, into the options dictionary.

## See Also

### Related Documentation

- apply:

Produces a object by applying a kernel function.

