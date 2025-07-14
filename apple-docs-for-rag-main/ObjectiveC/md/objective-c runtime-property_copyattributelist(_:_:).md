

- Objective-C Runtime
-  property_copyAttributeList(\_:\_:) 

Function

# property_copyAttributeList(\_:\_:)

Returns an array of property attributes for a given property.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func property_copyAttributeList(
    _ property: objc_property_t,
    _ outCount: UnsafeMutablePointer?
) -> UnsafeMutablePointer?
```

## Parameters 

`property`  

The property whose attributes you want to copy.

`outCount`  

The number of attributes returned in the array.

## Return Value

An array of property attributes. You must free the array with `free()`.

## See Also

### Working with Properties

func property_getName(objc_property_t) -> UnsafePointer&lt;CChar>

Returns the name of a property.

func property_getAttributes(objc_property_t) -> UnsafePointer&lt;CChar>?

Returns the attribute string of a property.

func property_copyAttributeValue(objc_property_t, UnsafePointer&lt;CChar>) -> UnsafeMutablePointer&lt;CChar>?

Returns the value of a property attribute given the attribute name.

