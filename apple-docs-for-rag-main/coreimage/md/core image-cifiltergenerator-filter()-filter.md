

- Core Image
- CIFilterGenerator
-  filter() 

Instance Method

# filter()

Creates a filter object based on the filter chain.

macOS 10.5+

``` source
func filter() -> CIFilter
```

## Return Value

A `CIFilter` object.

## Discussion

The topology of the filter chain is immutable, meaning that any changes you make to the filter chain are not reflected in the filter. The returned filter holds the export input and output keys.

