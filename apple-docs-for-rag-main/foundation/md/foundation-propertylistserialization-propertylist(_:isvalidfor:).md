

- Foundation
- PropertyListSerialization
-  propertyList(\_:isValidFor:) 

Type Method

# propertyList(\_:isValidFor:)

Returns a Boolean value that indicates whether a given property list is valid for a given format.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func propertyList(
    _ plist: Any,
    isValidFor format: PropertyListSerialization.PropertyListFormat
) -> Bool
```

## Parameters 

`plist`  

A property list object.

`format`  

A property list format. For possible values, see PropertyListSerialization.PropertyListFormat.

## Return Value

true if `plist` is a valid property list in format `format`, otherwise false.

