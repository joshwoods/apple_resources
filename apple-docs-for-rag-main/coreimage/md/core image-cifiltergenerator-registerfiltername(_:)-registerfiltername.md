

- Core Image
- CIFilterGenerator
-  registerFilterName(\_:) 

Instance Method

# registerFilterName(\_:)

Registers the name associated with a filter chain.

macOS 10.5+

``` source
func registerFilterName(_ name: String)
```

## Parameters 

`name`  

A unique name for the filter chain you want to register.

## Discussion

This method allows you to register the filter chain as a named filter in the Core Image filter repository. You can then create a `CIFilter` object from it using the the init(name:) method of the CIFilter class.

