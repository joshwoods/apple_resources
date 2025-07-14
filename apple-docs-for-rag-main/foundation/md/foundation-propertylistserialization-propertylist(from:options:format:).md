

- Foundation
- PropertyListSerialization
-  propertyList(from:options:format:) 

Type Method

# propertyList(from:options:format:)

Creates and returns a property list from the specified data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func propertyList(
    from data: Data,
    options opt: PropertyListSerialization.ReadOptions = [],
    format: UnsafeMutablePointer?
) throws -> Any
```

## Parameters 

`data`  

A data object containing a serialized property list.

`opt`  

The options used to create the property list. For possible values, see PropertyListSerialization.MutabilityOptions.

`format`  

Upon return, contains the format that the property list was stored in. Pass `nil` if you do not need to know the format.

## Return Value

A property list object corresponding to the representation in `data`. If data is not in a supported format, returns `nil`.

## Discussion

Handling Errors in Swift

In Swift, this method returns a nonoptional result and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

## See Also

### Deserializing a Property List

class func propertyList(with: InputStream, options: PropertyListSerialization.ReadOptions, format: UnsafeMutablePointer&lt;PropertyListSerialization.PropertyListFormat>?) throws -> Any

Creates and returns a property list by reading from the specified stream.

