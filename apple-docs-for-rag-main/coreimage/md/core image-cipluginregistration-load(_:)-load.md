

- Core Image
- CIPlugInRegistration
-  load(\_:) 

Instance Method

# load(\_:)

Loads and initializes an image unit, performing custom tasks as needed.

macOS 10.4+

``` source
func load(_ host: UnsafeMutableRawPointer!) -> Bool
```

**Required**

## Parameters 

`host`  

Reserved for future use.

## Return Value

Returns `true` if the image unit is successfully initialized

## Discussion

The `load` method is called once by the host to initialize the image unit when the first filter in the image unit is instantiated. The method provides the image unit with an opportunity to perform custom initialization, such as a registration check.

## See Also

### Related Documentation

Core Image Programming Guide

Image Unit Tutorial

