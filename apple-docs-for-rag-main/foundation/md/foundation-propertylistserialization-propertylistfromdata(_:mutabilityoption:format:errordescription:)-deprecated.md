

- Foundation
- PropertyListSerialization
-  propertyListFromData(\_:mutabilityOption:format:errorDescription:) Deprecated

Type Method

# propertyListFromData(\_:mutabilityOption:format:errorDescription:)

This method is deprecated. Use data(fromPropertyList:format:options:) instead.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
class func propertyListFromData(
    _ data: Data,
    mutabilityOption opt: PropertyListSerialization.MutabilityOptions = [],
    format: UnsafeMutablePointer?,
    errorDescription errorString: UnsafeMutablePointer?
) -> Any?
```

Deprecated

Use propertyList(from:options:format:) instead.

## Parameters 

`data`  

A data object containing a serialized property list.

`opt`  

The options used to create the property list. For possible values, see PropertyListSerialization.MutabilityOptions.

`format`  

If the property list is valid, upon return contains the format. `format` can be `nil`, in which case the property list format is not returned. For possible values, see PropertyListSerialization.PropertyListFormat.

`errorString`  

Upon return, if the conversion is successful, `errorString` is `nil`. If the conversion fails, upon return contains a string describing the nature of the error.

## Return Value

A property list object corresponding to the representation in `data`. If data is not in a supported format, returns `nil`.

## See Also

### Related Documentation

class func propertyList(from: Data, options: PropertyListSerialization.ReadOptions, format: UnsafeMutablePointer&lt;PropertyListSerialization.PropertyListFormat>?) throws -> Any

Creates and returns a property list from the specified data.

### Obsolete Methods

class func dataFromPropertyList(Any, format: PropertyListSerialization.PropertyListFormat, errorDescription: UnsafeMutablePointer&lt;NSString?>?) -> Data?

This method is obsolete and will be deprecated soon.

Deprecated

