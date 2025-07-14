

- Objective-C Runtime
-  property_copyAttributeValue(\_:\_:) 

Function

# property_copyAttributeValue(\_:\_:)

Returns the value of a property attribute given the attribute name.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func property_copyAttributeValue(
    _ property: objc_property_t,
    _ attributeName: UnsafePointer
) -> UnsafeMutablePointer?
```

## Parameters 

`property`  

The property whose value you are interested in.

`attributeName`  

A C string representing the name of the attribute.

## Return Value

The value string of the `attributeName` attribute, if one exists in `property`; otherwise, `nil`. You must free the returned value string with `free()`.

## See Also

### Working with Properties

func property_getName(objc_property_t) -> UnsafePointer&lt;CChar>

Returns the name of a property.

func property_getAttributes(objc_property_t) -> UnsafePointer&lt;CChar>?

Returns the attribute string of a property.

func property_copyAttributeList(objc_property_t, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;objc_property_attribute_t>?

Returns an array of property attributes for a given property.

