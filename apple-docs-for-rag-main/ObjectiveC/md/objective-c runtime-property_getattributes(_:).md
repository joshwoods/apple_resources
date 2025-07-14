

- Objective-C Runtime
-  property_getAttributes(\_:) 

Function

# property_getAttributes(\_:)

Returns the attribute string of a property.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func property_getAttributes(_ property: objc_property_t) -> UnsafePointer?
```

## Return Value

A C string containing the property’s attributes.

## Discussion

The format of the attribute string is described in Declared Properties in Objective-C Runtime Programming Guide.

## See Also

### Working with Properties

func property_getName(objc_property_t) -> UnsafePointer&lt;CChar>

Returns the name of a property.

func property_copyAttributeValue(objc_property_t, UnsafePointer&lt;CChar>) -> UnsafeMutablePointer&lt;CChar>?

Returns the value of a property attribute given the attribute name.

func property_copyAttributeList(objc_property_t, UnsafeMutablePointer&lt;UInt32>?) -> UnsafeMutablePointer&lt;objc_property_attribute_t>?

Returns an array of property attributes for a given property.

