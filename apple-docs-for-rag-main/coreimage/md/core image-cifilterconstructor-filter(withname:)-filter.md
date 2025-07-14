

- Core Image
- CIFilterConstructor
-  filter(withName:) 

Instance Method

# filter(withName:)

Returns a filter object specified by name.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func filter(withName name: String) -> CIFilter?
```

**Required**

## Parameters 

`name`  

The name of the requested custom filter.

## Return Value

A `CIFilter` object implementing the custom filter.

## Discussion

Core Image calls this method when a filter is requested by name using the `CIFilter` class method init(name:) method (or related methods). Your implementation of this method should provide a new instance of the `CIFilter` subclass for your custom filter.

## See Also

### Related Documentation

Core Image Programming Guide

