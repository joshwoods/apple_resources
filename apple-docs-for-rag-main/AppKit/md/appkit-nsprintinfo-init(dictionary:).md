

- AppKit
- NSPrintInfo
-  init(dictionary:) 

Initializer

# init(dictionary:)

Returns a printing information object initialized with the parameters in the specified dictionary.

macOS

``` source
init(dictionary attributes: [NSPrintInfo.AttributeKey : Any])
```

## Parameters 

`attributes`  

The possible key-value pairs contained in `aDictionary` are described in Constants.

## Return Value

An initialized `NSPrintInfo` object, or nil if the object could not be created.

## Discussion

This method is the designated initializer for this class. Non-object values should be stored in `NSValue` objects (or an appropriate subclass like `NSNumber`) in the dictionary. See NSNumber for a list of types which should be stored using the `NSNumber` class; otherwise use `NSValue`.

## See Also

### Related Documentation

Printing Programming Guide for Mac

func dictionary() -> NSMutableDictionary

Returns the print info’s dictionary that contains the printing attributes.

### Creating the Printing Information Object

class var shared: NSPrintInfo

The shared printing information object.

convenience init()

Creates a printing information object.

init(coder: NSCoder)

Creates a printing information object from data in an unarchiver.

