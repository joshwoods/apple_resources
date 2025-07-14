

- Core Image
- CIFilter
-  init(name:) 

Initializer

# init(name:)

Creates a `CIFilter` object for a specific kind of filter.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+

``` source
init?(name: String)
```

## Parameters 

`name`  

The name of the filter. You must make sure the name is spelled correctly, otherwise your app will run but not produce any output images. For that reason, you should check for the existence of the filter after calling this method.

## Return Value

A `CIFilter` object whose input values are undefined.

## Discussion

In macOS, after creating a filter with this method you must call setDefaults() or set parameters individually by calling setValue(_:forKey:). In iOS, the filter’s parameters are automatically set to default values.

## See Also

### Creating a Filter

init?(name: String, parameters: [String : Any]?)

Creates a `CIFilter` object for a specific kind of filter and initializes the input values.

### Related Documentation

Image Unit Tutorial

+ filterWithName:keysAndValues:

Creates a object for a specific kind of filter and initializes the input values with a `nil`-terminated list of arguments.

Core Image Filter Reference

Core Image Programming Guide

