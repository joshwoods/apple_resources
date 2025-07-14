

- Foundation
- PropertyListSerialization
-  data(fromPropertyList:format:options:) 

Type Method

# data(fromPropertyList:format:options:)

Returns an `NSData` object containing a given property list in a specified format.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func data(
    fromPropertyList plist: Any,
    format: PropertyListSerialization.PropertyListFormat,
    options opt: PropertyListSerialization.WriteOptions
) throws -> Data
```

## Parameters 

`plist`  

A property list object.

`format`  

A property list format. For possible values, see PropertyListSerialization.PropertyListFormat.

`opt`  

The `opt` parameter is currently unused. No options should be specified.

## Return Value

An `NSData` object containing `plist` in the format specified by `format`.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Related Documentation

Archives and Serializations Programming Guide

Property List Programming Guide

### Serializing a Property List

class func writePropertyList(Any, to: OutputStream, format: PropertyListSerialization.PropertyListFormat, options: PropertyListSerialization.WriteOptions, error: NSErrorPointer) -> Int

Writes a property list to the specified stream.

typealias WriteOptions

