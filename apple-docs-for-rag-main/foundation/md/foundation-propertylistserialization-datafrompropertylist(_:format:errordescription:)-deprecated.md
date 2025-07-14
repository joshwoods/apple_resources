

- Foundation
- PropertyListSerialization
-  dataFromPropertyList(\_:format:errorDescription:) Deprecated

Type Method

# dataFromPropertyList(\_:format:errorDescription:)

This method is obsolete and will be deprecated soon.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.0–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
class func dataFromPropertyList(
    _ plist: Any,
    format: PropertyListSerialization.PropertyListFormat,
    errorDescription errorString: UnsafeMutablePointer?
) -> Data?
```

Deprecated

Use data(fromPropertyList:format:options:) instead.

## Parameters 

`plist`  

A property list object.

`format`  

A property list format. For possible values, see PropertyListSerialization.PropertyListFormat.

`errorString`  

Upon return, if the conversion is successful, `errorString` is `nil`. If the conversion fails, upon return contains a string describing the nature of the error.

## Return Value

An `NSData` object containing `plist` in the format specified by `format`.

## Discussion

This method is obsolete and will be deprecated soon. Use data(fromPropertyList:format:options:) instead.

## See Also

### Related Documentation

class func data(fromPropertyList: Any, format: PropertyListSerialization.PropertyListFormat, options: PropertyListSerialization.WriteOptions) throws -> Data

Returns an `NSData` object containing a given property list in a specified format.

### Obsolete Methods

class func propertyListFromData(Data, mutabilityOption: PropertyListSerialization.MutabilityOptions, format: UnsafeMutablePointer&lt;PropertyListSerialization.PropertyListFormat>?, errorDescription: UnsafeMutablePointer&lt;NSString?>?) -> Any?

This method is deprecated. Use data(fromPropertyList:format:options:) instead.

Deprecated

