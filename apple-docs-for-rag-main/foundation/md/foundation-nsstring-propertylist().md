

- Foundation
- NSString
-  propertyList() 

Instance Method

# propertyList()

Parses the receiver as a text representation of a property list, returning an `NSString`, `NSData`, `NSArray`, or `NSDictionary` object, according to the topmost element.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func propertyList() -> Any
```

## Return Value

A property list representation of returning an `NSString`, `NSData`, `NSArray`, or `NSDictionary` object, according to the topmost element.

## Discussion

The receiver must contain a string in a property list format. For a discussion of property list formats, see Property List Programming Guide.

Important

Raises an `NSParseErrorException` if the receiver cannot be parsed as a property list.

## See Also

### Related Documentation

class func string(withContentsOfFile: String) -> Any?

Returns a string created by reading data from the file named by a given path.

Deprecated

### Converting String Contents Into a Property List

func propertyListFromStringsFileFormat() -> [AnyHashable : Any]?

Returns a dictionary object initialized with the keys and values found in the receiver.

